<template>
  <span class="von-badge">
    <div v-html="num" class="von-badge-num"></div>
  </span>
</template>
<style lang="scss" scoped>
  @import "../scss/variables";

  .von-badge {
    display: inline-block;
    padding: 3px 6px;
    height: 18px;
    z-index: 12;
    border-radius: 20px;
    background-color: $assertive;
    text-align: center;

    .von-badge-num {
      width: 100%;
      height: 12px;
      font-size: 12px;
      line-height: 12px;
      color: #FFF;
    }
  }
</style>
<script>
  import Scalable from '../scalable'

  export default {
    components: {
      Scalable
    },
    props: {
      num: String
    }
  }
</script>
