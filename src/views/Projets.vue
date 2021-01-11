<template>
  <div class="container flex flex-col mx-auto">
    <nav class="flex flex-row px-8 mt-10">
      <router-link to="" class="navigation-formations">Python</router-link>
      <router-link to="" class="navigation-formations">HTML</router-link>
      <router-link to="" class="navigation-formations">CSS</router-link>
    </nav>

    <div class="container flex flex-row flex-wrap justify-center mt-10">
      <Card title="test title #2" img="projets/scriptconnexioninstagram.png" link="#" />
      <Card title="test title #2" img="projets/scriptconnexioninstagram.png" link="#" />
      <Card title="test title #2" img="projets/scriptconnexioninstagram.png" link="#" />
      <Card title="test title #2" img="projets/scriptconnexioninstagram.png" link="#" />
    </div>
  </div>
</template>

<script>
import Card from '../components/card.vue';

export default {
  name: 'Projets',
  components: {
    Card
  }
}
</script>