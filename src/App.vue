<template>
  <div id="app">
    <div id="nav" class="flex flex-row">
      <router-link to="/about" class="navigation-link">A propos</router-link> |
      <router-link to="/formations" class="navigation-link">Formations</router-link> |
      <router-link to="/projets" class="navigation-link">Projets</router-link> |
      <router-link to="" class="navigation-link">CDB</router-link>

      <div class="absolute top-0 right-0 flex flex-row">
        <button class="navigation-btn" @click="isVisible = !isVisible" v-show="!isVisible">Follow me!</button>
        <a href="https://www.instagram.com/learn_computer_science/" target="_blank">
          <img src="../src/assets/img/instagram.png" alt="" class="px-2 h-10 mt-6" v-show="isVisible" >
        </a>
        <a href="https://www.youtube.com/channel/UCPsR5Z9laQtVkKy728gZQIQ?view_as=subscriber" target="_blank">
          <img src="../src/assets/img/youtube.png" alt="" class="px-2 h-10 mt-6" v-show="isVisible">
        </a>
        <router-link to="/">
          <img src="../src/assets/img/mainleve.png" alt="" class="h-20 px-2 py-2">
        </router-link>
        <!-- testing line -->
      </div>
    </div>
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      isVisible: false,
    }
  }
}
</script>

<style lang="scss">
html, body {
  background-color: #152634;
}

@font-face {
  font-family: "JetBrains Mono";
  src: url("/assets/Font/JetBrainsMono.ttf");
}

@font-face {
  font-family: "Zero Hour";
  src: url("/assets/Font/zerohour.ttf");
}

.navigation-link {
  @apply text-white hover:text-black hover:bg-white rounded px-2 py-0.5;
}

.navigation-btn {
  @apply text-white bg-primary px-2 h-10 mt-6 rounded mr-5 hover:text-black hover:bg-white;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50; //primary color
}

#nav {
  padding: 30px;
  background-color: #101E2A; //secondary color
  font-family: "JetBrains Mono", sans-serif;
}
</style>
