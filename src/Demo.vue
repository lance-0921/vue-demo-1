<template>
  <div class="red">
    {{ n }}
    <button @click="add">+1</button>
  </div>
</template>

<script>
export default {
  data() {
    //vue.loader的data只支持函數
    return {
      n: 0,
    };
  },
  methods: {
    add() {
      return (this.n += 1);
    },
  },
};
</script>

<style>
.red {
  color: red;
}
</style>
