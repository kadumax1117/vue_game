<template>
  <div>
    <Mondai v-bind:mondaibun="mondai1" />
    <Contents v-bind:message="sentakusi.A" />
    <Contents v-bind:message="sentakusi.B" />
    <Contents v-bind:message="sentakusi.C" />
    <Contents v-bind:message="sentakusi.D" />
  </div>
</template>

<script>
import Mondai from "./components/Mondai2.vue";
import Contents from "./components/Contents.vue"

export default {
  name: "App",
  components: {
    Mondai,
    Contents,
  },
  data() {
    return {
      mondai1:"好きな食べ物は？",
      sentakusi:{
        A:"おにぎり",
        B:"パスタ",
        C:"カレーライス",
        D:"唐揚げ"
      }
      // mon1:"おにぎり",
      // mon2:"カレー",
      // mon3:"パスタ",
      // mon4:"唐揚げ"
    }
  }
};
</script>