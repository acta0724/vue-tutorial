<script setup>
import { ref } from 'vue';

const fruits = ['りんご', 'バナナ', 'オレンジ'];

const selectedFruit = ref('');
</script>

<template>
  <v-card class="radio-example" title="好きな果物を選んでください">
    <v-card-text>
      <v-radio-group v-model="selectedFruit">
        <v-radio v-for="fruit in fruits" :key="fruit" :label="fruit" :value="fruit"></v-radio>
      </v-radio-group>

    <p v-if="selectedFruit">
      選択中の果物: <strong>{{ selectedFruit }}</strong>
    </p>
    <p v-else>
      まだ何も選択されていません。
    </p>
    </v-card-text>
  </v-card>
</template>

<style scoped>
.radio-example {
  margin-top: 20px;
  width: 300px;
}

.radio-example p {
  margin-top: 15px;
}

.radio-example :deep(.v-label) {
  font-size: 16px; /* お好みのサイズに変更してください (例: 16px) */
  opacity: 1; /* Vuetify 3.5.x以降で文字が薄くなる場合に追加 */
}
</style>