<template>
  <div class="container flex flex-col mx-auto">
    <SubNavigation />

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
import SubNavigation from '../components/sub-navigation.vue';
import Card from '../components/card.vue';

export default {
  name: 'formations',
  components: {
    SubNavigation,
    Card,
  }
}
</script>