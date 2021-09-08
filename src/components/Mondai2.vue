<template>
  <div class="mondaibun">
    {{ mondaibun }}
  </div>
</template>

<script>

export default {
  name: "Mondai2",
  props:{
    mondaibun:String,
  }
};
</script>
<style>
  .mondaibun {
    text-align: center;
    font-size: 30px;
  }
</style>
