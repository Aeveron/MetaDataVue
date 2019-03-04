<template>
  <div>
    <table>
      <tr v-for="row in rows">
        <td v-for="col in columns">
            {{ row[col] }}</td>
      </tr>
    </table>
  </div>
</template>

<script>
export default {
  data() {
    return {
     
    };
  },
  name: "Superform",
  methods: {},
  props:['Superform']
};
</script>

<style>
</style>
