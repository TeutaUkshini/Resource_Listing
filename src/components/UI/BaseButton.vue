<template>
  <button :class="mode">
    <slot></slot>
  </button>
</template>

<script>
export default {
  props: ['mode']
}
</script>

<style scoped>
button {
  padding: 0.75rem 1.5rem;
  font-family: inherit;
  background-color: #9b691f79;
  border: 1px solid #9b691f79;
  color: white;
  cursor: pointer;
}

button:hover,
button:active {
  background-color: #68625e;
  border-color: #68625e;
}

.flat {
  background-color: transparent;
  color: #000000;
  border: none;
}

.flat:hover,
.flat:active {
  background-color: #948b6d;
}
</style>