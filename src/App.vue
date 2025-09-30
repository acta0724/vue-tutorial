<template>
  <v-app>
    <v-main>
      <v-container>
        <div class="d-flex flex-column align-center">
          <RadioExample />
        </div>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
import RadioExample from './components/RadioExample.vue';

export default {
  name: 'App',
  components: {
    RadioExample
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
