<template>
  <div class="home container flex flex-col px-4 mx-auto xl:mt-20 xl:flex-row">
    <div class="max-w-2xl pt-20 mt-14 mx-auto">
      <h1 class="title text-white text-4xl">Bienvenue</h1>
      <h2 class="text text-white text-2xl">Sur le site Learn Computer Science</h2>
      <p class="text text-white mt-6 mb-10 text-sm">learn_computer_science, votre formateur, réalisateur de projets et
        accompagnant dans les domaines de la programmation, l'informatique, le bricolage, l'électronique, le
        business et pleins d'autre choses.
      </p>
      <button class="text text-white bg-secondary rounded px-4 py-2 hover:bg-white hover:text-black">En savoir plus...</button>
    </div>
    
    <div class="xl:mr-20">
      <img src="../assets/img/logoHome.png" alt="" class="mx-auto">
    </div>
  </div>
</template>

<script>
export default {
  name: 'Home',
  components: {},
}
</script>

<style lang="scss">
.title {
  font-family: "Zero Hour", sans-serif;
}

.text {
  font-family: "JetBrains Mono", sans-serif;
}
</style>
