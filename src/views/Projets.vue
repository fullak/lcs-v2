<template>
  <div class="container flex flex-col mx-auto">
    <SubNavigation />

    <div class="container flex flex-row flex-wrap justify-center mt-10">
      <Card title="test title #2" img="projets/scriptconnexioninstagram.png" link="#" />
      <Card title="test title #2" img="projets/scriptconnexioninstagram.png" link="#" />
      <Card title="test title #2" img="projets/scriptconnexioninstagram.png" link="#" />
      <Card title="test title #2" img="projets/scriptconnexioninstagram.png" link="#" />
    </div>
  </div>
</template>

<script>
import SubNavigation from '../components/sub-navigation.vue';
import Card from '../components/card.vue';

export default {
  name: 'Projets',
  components: {
    SubNavigation,
    Card
  }
}
</script>