<template>
  <div>
    <button @click="upFunction" class="btn btn-outline-info">up</button>
    <button @click="downFunction" class="btn btn-outline-info">down</button>
    <p v-bind:style="{ fontSize: fsize + 'px' }" class="text-info">LOVE_SANRIO</p>
  </div>
</template>

<script>
export default {
  data: function () {
    return {
      counter: 0,
      fsize:100,
    };
  },
  props: {
    lable: String,
  },
  methods: {
    upFunction: function () {
      this.fsize += 10;
      console.log("fsize = " + this.fsize);
    },
    downFunction: function () {
      this.fsize -= 10;
      console.log(this.fsize);
    },
  },
};
</script> 
<style>
</style>