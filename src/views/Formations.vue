<template>
  <div class="container flex flex-col mx-auto">
    <nav class="flex flex-row px-8 mt-10">
      <router-link to="" class="navigation-formations">Python</router-link>
      <router-link to="" class="navigation-formations">HTML</router-link>
      <router-link to="" class="navigation-formations">CSS</router-link>
    </nav>

    <div class="container flex flex-row flex-wrap justify-center mt-10">
      <Card title="test this shit!" img="pythonfeatured.jpg" link="http://www.google.com/"/>
      <!-- <Card title="test title #2" img="projets/scriptconnexioninstagram.png" link="#" /> -->
      <Card title="test this shit 2!" img="pythonfeatured.jpg" link="http://www.google.com/"/>
      <Card title="a title!" img="pythonfeatured.jpg" link="http://www.google.com/"/>
      <Card title="this guy is incredible!" img="pythonfeatured.jpg" link="http://www.google.com/"/>
      <Card title="OMFG!" img="pythonfeatured.jpg" link="http://www.google.com/"/>
      <Card title="hi there!" img="pythonfeatured.jpg" link="http://www.google.com/"/>
    </div>
  </div>
</template>

<script>
import Card from '../components/card.vue';

export default {
  name: 'formations',
  components: {
    Card,
  }
}
</script>

<style lang="scss">
.navigation-formations {
  @apply mr-6 border border-white text-white rounded px-8 py-0.5 text-xl hover:text-black hover:bg-white;
  font-family: "JetBrains Mono", sans-serif;
}
</style>