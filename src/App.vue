<template>
  <div id="App" :style="image" class="bg-image">
    <images></images>
  </div>
</template>

<script>
import images from "./components/componentes.vue";

export default {
  name: "App",
  components: {
    images,
  },
  data() {
    return {
      image: {
        backgroundImage:
          "url(https://rickandmortypod.com/wp-content/uploads/2018/11/cropped-RM_page-header_background1-3.png)",
      },
    };
  },
};
</script>

<style scoped>
.bg-image {
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
}
</style>