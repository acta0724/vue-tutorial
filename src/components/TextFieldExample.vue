<script setup>
import { ref } from 'vue';

const name = ref('');
</script>

<template>
  <v-card class="text-field-example" title="テキストフィールドの例">
    <v-card-text>
      <v-text-field
        v-model="name"
        label="名前を入力してください"
        clearable
        disabled="false"
      ></v-text-field>

      <p v-if="name">
        入力された名前: <strong>{{ name }}</strong>
      </p>
      <p v-else>
        入力まだだよー
      </p>
    </v-card-text>
  </v-card>
</template>

<style scoped>
.text-field-example {
  margin-top: 20px;
  width: 300px;
}

.text-field-example p {
  margin-top: 15px;
}
</style>