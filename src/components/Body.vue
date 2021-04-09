<template>
  <div>
    <div class="container">
      <div v-if="state"><img src="../assets/source.gif" /></div>
      <div id="off" v-else></div>
    </div>
    <button class="btn btn-primary-danger" v-on:click="changeState">
      <span v-if="state"> Off</span>
      <span v-else>On</span>
    </button>
  </div>


  <div>
<h3>Student Registration</h3>
<ol></ol>
  </div>
</template>

<script>
export default {
  name: 'Body',
  data: function () {
    return {
      state: false,
    };
  },

  methods: {
    changeState: function () {
      this.state = !this.state;
    },
  },
};
</script>

<style scoped>
.container {
  width: 420px;
  align-content: center;
  background-color: rgb(10, 10, 10);
  width: 500px;
  height: 500px;
  border: 15px solid rgb(11, 12, 11);
  margin: center;
  background-size: cover;
  border-radius: 10px;
}

button {
  position: relative;
  margin-top: -70px;
  border-radius: 100%;
  transition: 0.5s;
  border: 1px solid red;
}
img {
  background: center;
  position: relative;
  width: 420px;
}
</style>
