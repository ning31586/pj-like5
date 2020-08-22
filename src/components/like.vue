<template>
  <div>
    <div class="row-12">
      <button @click="Like()" class="btn btn-outline-info">
        <i class="fa fa-thumbs-o-up" aria-hidden="true"></i> Like
      </button>
      <button @click="Dislike()" class="btn btn-outline-info">
        <i class="fa fa-thumbs-o-down" aria-hidden="true"></i> Dislike
      </button>
      <button @click="Love()" class="btn btn-outline-info">
        <i class="fa fa-heart-o" aria-hidden="true"></i> Love
      </button>
      <button @click="Sad()" class="btn btn-outline-info">
        <i class="fa fa-frown-o" aria-hidden="true"></i> Sad
      </button>
      <button @click="reset()" class="btn btn-outline-info">
        <i class="fa fa-refresh" aria-hidden="true"></i> reset
      </button>
      <br />
      <br />
      <p v-bind:style="{fontSize: fonts + 'px' }">{{ counter }}</p>
    </div>
  </div>
</template>

<script>
export default {
  data: function () {
    return {
      counter: 0,
      fonts: 50,
    };
  },
  methods: {
    Like: function () {
      this.counter += 1;
      console.log(this.counter);
    },
    Dislike: function () {
      this.counter -= 5;
      console.log(this.counter);
    },
    Love: function () {
      this.counter += 5;
      console.log(this.counter);
    },
    Sad: function () {
      this.counter -= 1;
      console.log(this.counter);
    },
    reset: function () {
      this.counter = 0;
      console.log(this.counter);
    },
  },
};
</script>


<style>
</style>