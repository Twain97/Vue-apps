<template>
  <div>
    <Header />
    <ProfilePage />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import ProfilePage from "./components/ProfilePage.vue";

export default {
  name: "App",
  components: { Header, ProfilePage },
};
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  background-color: rgb(11, 2, 17);
}
</style>
