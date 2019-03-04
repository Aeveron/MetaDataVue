<template>
  <div>
    <super-form v-bind:metadata="mySuperform.metadata" v-bind:data="mySuperform.data" />
    <hr>

  </div>
</template>

<script>
import Superform from '@/components/Superform';

export default {
  data() {
    return {
      mySuperform: {
        metadata: {
          columns: ["name", "birthyear", "sex"]
        },
        data: {
          name: "Terje",
          birthyear: 1975,
          sex: "male",       
        }
      }
    }
  },
  components: {
    SuperForm: Superform
  }
};
</script>

<style scoped>
</style>

