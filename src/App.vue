<template>
  <div id="app">
    <div id="nav">
      <router-link :to="{ name: 'event-create' }">Create Event</router-link>
      <router-link :to="{ name: 'event-list' }">List Event</router-link>
      <router-link :to="{ name: 'event-show' }">Show Event</router-link>
    </div>

    <router-view />
  </div>
</template>

<script>
export default {
  name: 'app'
};
</script>
<style lang="stylus" scoped>
#app{
  width: 100%;
  padding: 50px 200px 50px 200px;
}
#nav{
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
  width: 400px;
}
a:link {
  text-decoration: none;
}
</style>
