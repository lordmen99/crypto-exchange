<template>
  <div class="currenc-container-split">
    <p>{{ currenc }} {{ balance }}</p>
    <button @click="$emit('toggle-input')">Ввод</button>
    <button @click="$emit('toggle-output')">Вывод</button>
  </div>
</template>
<script>
export default {
  name: "CurrencButton",
  props: {
    currenc: { required: true, type: String },
    balance: { required: true, type: Number },
  },
};
</script>
