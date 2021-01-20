<template>
  <div class="container flex flex-col mx-auto">
    <SubNavigation />

    <Modal v-show="displayModal" @close="displayModal = false"/>

    <div class="container flex flex-row flex-wrap justify-center mt-10">
      <Card title="test this shit!" img="pythonfeatured.jpg" @click.native="displayModal = !displayModal" />
      <!-- <Card title="test title #2" img="projets/scriptconnexioninstagram.png" link="#" /> -->
      <Card title="test this shit!" img="pythonfeatured.jpg" @click.native="displayModal = !displayModal" />
      <Card title="test this shit!" img="pythonfeatured.jpg" @click.native="displayModal = !displayModal" />
      <Card title="test this shit!" img="pythonfeatured.jpg" @click.native="displayModal = !displayModal" />
      <Card title="test this shit!" img="pythonfeatured.jpg" @click.native="displayModal = !displayModal" />
      <Card title="test this shit!" img="pythonfeatured.jpg" @click.native="displayModal = !displayModal" />
      <Card title="test this shit!" img="pythonfeatured.jpg" @click.native="displayModal = !displayModal" />
    </div>
  </div>
</template>

<script>
import SubNavigation from '../components/sub-navigation.vue';
import Card from '../components/card.vue';
import Modal from '../components/formations-modal.vue';

export default {
  name: 'formations',
  components: {
    SubNavigation,
    Card,
    Modal,
  },
  data () {
    return {
      displayModal: false,
    }
  }
}
</script>