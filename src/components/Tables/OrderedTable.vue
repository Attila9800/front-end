<template>
  <div>
    <md-table v-model="users" :table-header-color="tableHeaderColor">
      <md-table-row slot="md-table-row" slot-scope="{ item }">
        <md-table-cell md-label="ID">{{ item.id }}</md-table-cell>
        <md-table-cell md-label="Name">{{ item.name }}</md-table-cell>
        <md-table-cell md-label="Salary">{{ item.salary }}</md-table-cell>
        <md-table-cell md-label="Country">{{ item.country }}</md-table-cell>
        <md-table-cell md-label="City">{{ item.city }}</md-table-cell>
      </md-table-row>
    </md-table>
  </div>
</template>

<script>
export default {
  name: "ordered-table",
  props: {
    tableHeaderColor: {
      type: String,
      default: ""
    }
  },
  data() {
    return {
      selected: [],
      users: [
        {
          id: 1,
          name: "叶得力",
          salary: "$46,738",
          country: "哈萨克斯坦",
          city: "阿斯塔纳"
        },
        {
          id: 2,
          name: "伊万",
          salary: "$33,738",
          country: "俄罗斯",
          city: "莫斯科"
        },
        {
          id: 3,
          name: "胡萨",
          salary: "$20,142",
          country: "孟加拉",
          city: "达卡"
        },
        {
          id: 4,
          name: "小韩",
          salary: "$18,735",
          country: "Korea, South",
          city: "首尔"
        }
      ]
    };
  }
};
</script>
