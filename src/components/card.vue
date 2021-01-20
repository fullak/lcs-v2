<template>
  <a href="#" class="container w-80 ml-2 mr-2 mt-4">
    <img :src="require(`@/assets/img/${img}`)" alt="" class="">
    <h2 class="text text-white bg-primary text-md px-1">{{ title }}</h2>
  </a>
</template>

<script>
export default {
  name: 'card',
  props: [
    "img",
    "title"
  ],
}
</script>