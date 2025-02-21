<script setup>
import { RouterLink, RouterView } from 'vue-router'
import { reactive } from 'vue';
// defineProps({
//   aaa: {
//     type: String,
//     default: "home",
//   },
// })
const form = reactive({
  Email: '',
  Passwword: ''
})

const login = async () => {
  console.log(form.Email);
};

</script>

<template>
    <form @submit.prevent="login">
      <label for="e-mail">Enter E-mail</label>
      <input v-model="form.Email" id="e-mail" required>
      <label for="passwword">Enter passwword</label>
      <input v-model="form.Passwword" id="passwword" required>
      <button type="submit">Log in</button>
    </form>
  
</template>

<style scoped>
input[type=text], select {
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  display: inline-block;
  border: 1px solid #ccc;
  border-radius: 4px;
  box-sizing: border-box;
}

input[type=submit] {
  width: 100%;
  background-color: #4CAF50;
  color: white;
  padding: 14px 20px;
  margin: 8px 0;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

input[type=submit]:hover {
  background-color: #45a049;
}

div {
  border-radius: 5px;
  background-color: #f2f2f2;
  padding: 20px;
}
.s::placeholder {
  background-color: rgb(120, 120, 255);
}
</style>
