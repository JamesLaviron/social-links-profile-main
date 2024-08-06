<template>
  <a :href="url" class="network-link text-preset-2-bold">
    {{ content }}
  </a>
</template>

<script>
export default {
  name: "NetworkLink",
  props: {
    content: String,
    url: String,
  },
};
</script>

<style scoped>
.network-link {
  color: white;
  border-radius: 0.8rem;
  padding: var(--spacing-150);
  gap: var(--spacing-100);
  background-color: var(--color-grey-700);
  text-decoration-line: none;
}

.network-link:hover {
  background-color: var(--color-green);
}
</style>
