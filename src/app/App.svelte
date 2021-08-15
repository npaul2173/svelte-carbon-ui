<script>
  import "carbon-components-svelte/css/all.css";
  import router from "page";
  import Dashboard from "../dashboard/dashboard.svelte";
  import Orders from "../orders/orders.svelte";
  import Header from "../common/components/Header/header.svelte";
  import ThemeManager from "../common/components/Theme/theme.svelte";
  let page;

  // let theme = "white"; // "white" | "g10" | "g80" | "g90" | "g100"
  // $: document.documentElement.setAttribute("theme", theme);

  router("/", () => (page = Dashboard));
  router("/Orders", () => (page = Orders));

  router.start();
</script>

<Header />
<svelte:component this={page} />

<style>
  :global(body) {
    padding: 0;
    margin: 0;
    box-sizing: border-box;
  }
</style>
