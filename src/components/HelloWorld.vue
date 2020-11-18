<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h1>{{ title }}</h1>
    <input type="text" v-model="title" />
    <br />
    <p v-if="show">You can see me!</p>
    <p v-show="show">You can see me using SHOW</p>
    <button @click="show = !show">Toggle Show</button>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: {
      type: String,
    },
  },
  data() {
    return {
      title: "",
      show: true,
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
