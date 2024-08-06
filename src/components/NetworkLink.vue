<!-- create a vue component that takes content and url and renders a styled link to the url with the content as the text -->

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
  color: var(--color-grey-700);
  border-radius: 0.8rem;
  padding: var(--spacing-150);
  gap: var(--spacing-100);
}

.network-link:hover {
  background-color: var(--color-green-100);
}
</style>
