<template>
  <div id="app">
    <img class="rounded-circle" src="./assets/7.jpg" width="50%" />
    <br><br><br>
    <HelloWorld msg="SANRIO"   />
    <br>
    <hr />
    <br><br><br>
    <div class="row">
      <div class="col">
        <img class="rounded border border-dark" src="./assets/1.png" width="60%" />
        <br />
        <br />
        <coun />
      </div>
      <div class="col">
        <img class="rounded border border-dark" src="./assets/2.png" width="60%" />
        <br />
        <br />
        <coun />
      </div>
      <div class="col">
        <img class="rounded border border-dark" src="./assets/3.png" width="60%" />
        <br />
        <br />
        <coun />
      </div>
    </div>
    <div class="row">
      <div class="col">
        <img class="rounded border border-dark" src="./assets/4.png" width="60%" />
        <br />
        <br />
        <coun />
      </div>
      <div class="col">
        <img class="rounded border border-dark" src="./assets/5.png" width="60%" />
        <br />
        <br />
        <coun />
      </div>
      <div class="col">
        <img class="rounded border border-dark" src="./assets/6.png" width="60%" />
        <br />
        <br />
        <coun />
      </div>
    </div>
    <br>
    <hr />
    <br><br><br>
    <div class="row">
    <br><hr /><br><br><br><br><br>
      <div class="col">
        
        <fonts />
        <hr />
        <div class="row-12">
          ชื่อ-นามสกุล
          <input type="text" v-model="name" />
          รหัสนักศึกษา
          <input type="number" v-model="code" />
          GPA
          <input type="number" v-model="gpa" step="0.1" />
          <br />
          <br />
        </div>
        <div class="row-12">แสดง:ชื่อ {{name}}  รหัสนักศึกษา {{code}} GPA {{gpa}}</div>
        <br />
        <br />
      </div>
    </div>
    <footer class="my-5 pt-5 text-muted text-center text-small">
        <p class="mb-1">&copy; cs313@6104101352</p>
    </footer>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import coun from "./components/like.vue";
import fonts from "./components/fonts.vue";
export default {
  name: "App",
  components: {
    HelloWorld,
    coun,
    fonts,
  },
  data: function () {
    return {
      total: 0,
      name: "",
      code: "",
      gpa: 0.1,
    };
  },
};
</script>




<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #241602;
  margin-top: 50px;
}
</style>
