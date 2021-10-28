<template>
  <div class="container">
    <Header />
    <div class="user-input">
      <input 
      placeholder="Press enter team name"
      v-model="input" />
      <button @click="searchTeam">Search Team</button>
    </div>
  </div>

</template>

<script>
import Header from './components/Header.vue'
export default {
  components: {
    Header
  }
}
</script>

<style lang="scss">

.container {
  max-width: 600px;
  margin: 80px auto;
}

.user-input {
  display: flex;
  align-items: center;
  padding-bottom: 20px;
  input {
    width: 100%;
    padding: 10px 6px;
    margin-right: 10px;
  }
}

  button {
  appearance: none;
  padding: 10px;
  font-weight: bold;
  border-radius: 10px;
  border: none;
  background: grey;
  color: white;
  white-space: nowrap;

  + button {
    margin-left: 10px;
  }
}

</style>