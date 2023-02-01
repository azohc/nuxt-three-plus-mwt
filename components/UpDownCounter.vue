<template>
  <h1>
    {{ count }}
  </h1>
  <div>
    <button @click="increaseCount">up</button>
    <button @click="decreaseCount">down</button>
  </div>
</template>

<script setup lang="ts">
const count = ref<number>(0);

function increaseCount() {
  count.value += 1;
}

function decreaseCount() {
  count.value -= 1;
}
</script>
