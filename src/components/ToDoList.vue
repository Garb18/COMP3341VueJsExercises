<template>
  <div class="ToDoList">
    <ul>
      <li v-for="(ingredient, index) in ingredients" :key="index">
        {{ ingredient.message }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "ToDoList",
  props: {},
  data() {
    return {
      ingredients: [
        { message: "apples" },
        { message: "butter" },
        { message: "milk" },
      ],
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
body {
  background-color: #ececec;
}
</style>
