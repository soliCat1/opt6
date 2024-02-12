<template>
  <section>
    <ag-grid-vue
    :row-height="45"
    class="ag-theme-alpine"
    style="height: 500px"
    :columnDefs="columnDefs"
    :rowData="rowData"></ag-grid-vue>
  </section>
</template>

<script>
import { AgGridVue } from "ag-grid-vue3";
import 'ag-grid-community/styles/ag-grid.css'
import 'ag-grid-community/styles/ag-theme-alpine-no-font.css'

export default {
  name: 'table-section',
  components: {
    AgGridVue
  },
  setup(){
    return {
      columnDefs: [
        {field: 'Наименование еденицы',
        cellStyle: {borderRadius: '5px', border: 'solid 1px #ccc', padding: '8px 15px 9px 15px', margin: '5px 0', height: '35px'}},
        {field: 'Цена',
        cellStyle: {borderRadius: '5px', border: 'solid 1px #ccc', padding: '8px 15px 9px 15px', margin: '5px 0', height: '35px'}},
        {field: 'Кол-во',
        cellStyle: {borderRadius: '5px', border: 'solid 1px #ccc', padding: '8px 15px 9px 15px', margin: '5px 0', height: '35px'}},
        {field: 'Название товара',
        cellStyle: {borderRadius: '5px', border: 'solid 1px #ccc', padding: '8px 15px 9px 15px', margin: '5px 0', height: '35px'}},
        {field: 'Итого',
        cellStyle: {borderRadius: '5px', border: 'solid 1px #ccc', padding: '8px 15px 9px 15px', margin: '5px 0', height: '35px'}
    }
      ],
      rowData: [
        {'Наименование еденицы': 'Мраморный щебень фр. 2-5 мм, 25кг', 'Цена': 1231, 'Кол-во': 12, 'Название товара': 'Мраморный щебень', 'Итого': 1231},
        {'Наименование еденицы': 'Мраморный щебень фр. 2-5 мм, 25кг', 'Цена': 1231, 'Кол-во': 12, 'Название товара': 'Мраморный щебень', 'Итого': 1231},
        {'Наименование еденицы': 'Мраморный щебень фр. 2-5 мм, 25кг', 'Цена': 1231, 'Кол-во': 12, 'Название товара': 'Мраморный щебень', 'Итого': 1231}
      ]
    }
  }
}
</script>

<style scoped lang="scss">
section {
  padding: 32px 0 45px 0;
  border-radius: 10px;
  box-shadow: 0 5px 20px 0 rgba(0, 0, 0, 0.07);
  border: solid 1px #eeeff1;
  background-color: #ffffff;
}

.ag-theme-alpine {
    --ag-font-family: inherit;
    --ag-border-radius: none;
    --ag-borders: none;
    --ag-cell-horizontal-padding: 8px;
    --ag-grid-size: 2px;
    --ag-row-height: 20px;
    --ag-list-item-height: 400px;
    border-top: 1px solid #eeeff1;
}
</style>