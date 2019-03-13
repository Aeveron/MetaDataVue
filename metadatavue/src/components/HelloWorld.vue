<template>
  <div>
    <super-form :SuperForm="this.mySuperform"/>
    <hr>
  </div>
</template>

<script>
import Superform from "@/components/Superform";

export default {
  data() {
    return {
      mySuperform: {
        metadata: {
          columns: ["name", "birthyear", "sex", "country", "sivil status", "siblings"]
        },
        data: [
          {
            name: "Terje",
            birthyear: 1975,
            country: "NO",
            sex: "male"
          },
          {
            name: "Kristoffer",
            birthyear: 1994,
            sex: "male",
            country: "NO"
          },
          {
            name: "Emil",
            birthyear: 6969,
            sex: "attackhelicopter",
            country: "north korea"
          }
        ]
      }
    };
  },
  components: {
    SuperForm: Superform
  }
};
</script>

<style scoped>
</style>