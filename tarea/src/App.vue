<template>
  <MenuComponent/>
  <BodyComponent/>
  <FooterComponent/>
</template>

<script>
import MenuComponent from './components/MenuComponent.vue';
import BodyComponent from './components/BodyComponent.vue';
import FooterComponent from './components/FooterComponent.vue';

export default {
  name: 'App',
  components: {
    MenuComponent,
    BodyComponent,
    FooterComponent
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
