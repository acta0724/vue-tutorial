<template>
  <v-app>
    <v-main>
      <v-container>
        <div class="d-flex flex-column align-center">
          <RadioExample />
          <TextFieldExample />
        </div>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
import RadioExample from './components/RadioExample.vue';
import TextFieldExample from './components/TextFieldExample.vue';

export default {
  name: 'App',
  components: {
    RadioExample,
    TextFieldExample
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
