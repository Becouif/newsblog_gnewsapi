<template>
  <the-header></the-header>
  <blog-post></blog-post>
</template>

<script>
import TheHeader from "./components/TheHeader.vue";
import BlogPost from "./components/BlogPost.vue";
export default {
  components: { TheHeader,BlogPost },
  data() {
    return {};
  },
};
</script>

<style>
html {
  min-height: 100%;
  position: relative;
}
</style>
