<script>
  import {
    Button,
    Checkbox,
    Column,
    Content,
    DataTable,
    Form,
    FormGroup,
    RadioButton,
    RadioButtonGroup,
    Row,
    Select,
    SelectItem,
  } from "carbon-components-svelte";
</script>

<!-- <div class="container">
  <h1>Orders</h1>
</div> -->

<div class="container">
  <Content>
    <Column>
      <DataTable
        headers={[
          { key: "name", value: "Name" },
          { key: "protocol", value: "Protocol" },
          { key: "port", value: "Port" },
          { key: "rule", value: "Rule" },
        ]}
        rows={[
          {
            id: "a",
            name: "Load Balancer 3",
            protocol: "HTTP",
            port: 3000,
            rule: "Round robin",
          },
          {
            id: "b",
            name: "Load Balancer 1",
            protocol: "HTTP",
            port: 443,
            rule: "Round robin",
          },
          {
            id: "c",
            name: "Load Balancer 2",
            protocol: "HTTP",
            port: 80,
            rule: "DNS delegation",
          },
          {
            id: "d",
            name: "Load Balancer 6",
            protocol: "HTTP",
            port: 3000,
            rule: "Round robin",
          },
          {
            id: "e",
            name: "Load Balancer 4",
            protocol: "HTTP",
            port: 443,
            rule: "Round robin",
          },
          {
            id: "f",
            name: "Load Balancer 5",
            protocol: "HTTP",
            port: 80,
            rule: "DNS delegation",
          },
        ]}
      />
    </Column>
    <Column>
      <Form on:submit>
        <FormGroup legendText="Checkboxes">
          <Checkbox id="checkbox-0" labelText="Checkbox Label" checked />
          <Checkbox id="checkbox-1" labelText="Checkbox Label" />
          <Checkbox id="checkbox-2" labelText="Checkbox Label" disabled />
        </FormGroup>
        <FormGroup legendText="Radio buttons">
          <RadioButtonGroup
            name="radio-button-group"
            selected="default-selected"
          >
            <RadioButton
              id="radio-1"
              value="standard"
              labelText="Standard Radio Button"
            />
            <RadioButton
              id="radio-2"
              value="default-selected"
              labelText="Default Selected Radio Button"
            />
            <RadioButton
              id="radio-4"
              value="disabled"
              labelText="Disabled Radio Button"
              disabled
            />
          </RadioButtonGroup>
        </FormGroup>
        <FormGroup>
          <Select
            id="select-1"
            labelText="Select menu"
            value="placeholder-item"
          >
            <SelectItem
              disabled
              hidden
              value="placeholder-item"
              text="Choose an option"
            />
            <SelectItem value="option-1" text="Option 1" />
            <SelectItem value="option-2" text="Option 2" />
            <SelectItem value="option-3" text="Option 3" />
          </Select>
        </FormGroup>
        <Button type="submit">Submit</Button>
      </Form>
    </Column>
  </Content>
</div>

<style>
  /* .container {
    background-color: aquamarine;
  } */
</style>
