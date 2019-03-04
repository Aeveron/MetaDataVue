<template>
  <div>
    <b-row>
      <b-col md="12">
        <div class="table-responsive">
          <table class="table table-striped">
            <thead>
              <tr>
                <!-- eslint-disable -->
                <th v-for="Header in SuperForm.metadata.columns">{{Header}}</th>
              </tr>
            </thead>
            <tbody>
              <tr v-for="Data in SuperForm.data">
                <td v-for="Header in SuperForm.metadata.columns">{{Data[Header]}}</td>
              </tr>
            </tbody>
          </table>
        </div>
      </b-col>
    </b-row>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
  name: "Superform",
  methods: {},
  props: ["SuperForm"]
};
</script>

<style>
</style>