<template>
  <nav class="flex flex-row px-8 mt-10">
    <router-link to="" class="navigation-formations">Python</router-link>
    <router-link to="" class="navigation-formations">HTML</router-link>
    <router-link to="" class="navigation-formations">CSS</router-link>
  </nav>
</template>

<script>
export default {
  name: 'sub-navigation'
}
</script>

<style lang="scss">
.navigation-formations {
  @apply mr-6 border border-white text-white rounded px-8 py-0.5 text-xl hover:text-black hover:bg-white;
  font-family: "JetBrains Mono", sans-serif;
}
</style>