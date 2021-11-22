<template>
  <div class="outer-shell">
    <Header></Header>
    <Main></Main>
    <Footer></Footer>
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import Main from '@/components/Main.vue'
import Footer from '@/components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer,
  }
}
</script>

<style lang="scss">
@import 'styles/variables';
@import 'styles/header';
@import 'styles/main';
@import 'styles/footer';
@import 'styles/utilities';
@import "~bootstrap/scss/bootstrap";
@import "~font-awesome/css/font-awesome.css";

</style>
