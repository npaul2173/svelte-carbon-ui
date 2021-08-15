<script>
  import { Content, Row } from "carbon-components-svelte";

  import page from "page";

  const handleonClick = () => {
    page("./Orders");
  };
</script>

<div class="container">
  <Content>
    <h1>Dashboard</h1>
    <Row />
  </Content>
</div>

<style>
</style>
