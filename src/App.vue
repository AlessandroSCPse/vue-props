<template>
  <div id="app">
    
    <TitleComponent titleText="Mio testo" />

    <BannerComponent v-for="banner, index in banners" :key="index" :bannerDetails="banner" />
  </div>
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";
import TitleComponent from "./components/TitleComponent.vue";
import BannerComponent from "./components/BannerComponent.vue";

export default {
  name: "App",
  data() {
    return {
      titleTextOne: 'Ciao sono il primo componente',
      banners: [
        {
          title: 'Mare',
          img: 'https://www.tuscanypeople.com/wp-content/uploads/2021/07/spiaggia_sansone_elba.jpg'
        },
        {
          title: 'Montagna',
          img: 'https://siviaggia.it/wp-content/uploads/sites/2/2020/04/vette-italia.jpg'
        }
      ],
    };
  },
  components: {
    TitleComponent,
    BannerComponent
    // HelloWorld,
  },
};
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

img {
  width: 100%;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
