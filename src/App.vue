<template>
  <div id="app">
    <Header title="WasshoiHouse" />
    <form id="join-form">
      <div class="item">
        <p>User ID</p>
        <input id="userId" type="text" placeholder="" required />
      </div>
      <div class="item">
        <p>Account Name</p>
        <input id="accountName" type="text" placeholder="" required />
      </div>
      <div class="button-group">
        <b-button
          id="join"
          type="submit"
          class="item"
          size="lg"
          variant="primary"
        >
          Join
        </b-button>
        <b-button class="item" size="lg" variant="secondary">
          Create Room
        </b-button>
      </div>
    </form>
  </div>
</template>

<script>
import Header from "./components/Header.vue";

export default {
  name: "App",
  components: {
    Header,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.item {
  margin: 10px 0;
}

.button-group > .item {
  margin: 15px;
}
</style>
