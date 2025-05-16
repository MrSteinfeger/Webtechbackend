<template>
  <div>
    <h1>Baos wundervolle Computer</h1>
    <ItemList :items="computerListe" />
  </div>
</template>

<script>
import ItemList from "./components/ItemList.vue";

export default {
  name: "App",
  components: {
    ItemList,
  },
  data() {
    return {
      computerListe: ["Computer 1", "Computer 2", "Computer 3"],
    };
  },
};
</script>

<style scoped>
h1 {
  font-family: Arial, sans-serif;
  color: #2c3e50;
  text-align: center;
}
</style>
