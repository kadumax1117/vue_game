<template>
  <div v-on:click="doAction">
    <p class="sentakusi">{{ message }}</p>
  </div>
</template>

<script>
export default {
  name: "Contents",
  props: {
    message: String,
  },
  methods: {
    // thisは「このコンポーネント（にある）」
    doAction() {
      // console.log(this.message)
      if (this.message === "唐揚げ") {
        console.log("正解");
      } else {
        console.log("不正解");
      }
    },
  },
};
</script>
<style>
  .sentakusi {
    text-align: center;
    margin-top: 50px;
    font-size: 20px;
  }
</style>

