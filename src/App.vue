<template>
  <div id="app">
    <!-- HEADER -->
    <Header />
    <!-- MAIN -->
    <Main />
    <!-- INFO -->
    <section>
      <Info />
    </section>
    <!-- FOOTER -->
    <Footer />
    
  </div>
</template>

<script>
import Header from '@/components/Header.vue';
import Main from '@/components/Main.vue';
import Info from '@/components/Info.vue';
import Footer from '@/components/Footer.vue';

export default {
  name: 'App',
  components: {
      Header,
      Main,
      Info,
      Footer,

      
  }
}
</script>

<style>
    /* GENERAL */
    * {
      padding: 0;
      margin: 0;
      box-sizing: border-box;
      
    }

    body {
      font-family: 'Antonio', sans-serif;
      
    }
</style>
