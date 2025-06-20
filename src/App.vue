<template>
  <div>
    <h1>Daten vom Backend:</h1>
    <p v-if="data">{{ data.name }} ist {{ data.age }} Jahre alt</p>
    <p v-else>Lade Daten...</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      data: null
    }
  },
  mounted() {
    fetch("https://baobaowebtech.onrender.com") 
      .then(res => res.json())
      .then(data => this.data = data)
  }
}
</script>
