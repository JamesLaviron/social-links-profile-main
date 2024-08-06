<template>
  <div class="network-links">
    <NetworkLink content="GitHub" url="https://network-link.test" />
    <NetworkLink content="Frontend Mentor" url="https://network-link.test" />
    <NetworkLink content="LinkedIn" url="https://network-link.test" />
    <NetworkLink content="Twitter" url="https://network-link.test" />
    <NetworkLink content="Instagram" url="https://network-link.test" />
  </div>
</template>

<script>
import NetworkLink from "./NetworkLink.vue";
export default {
  name: "NetworkLinksList",
  components: {
    NetworkLink,
  },
};
</script>

<style scoped>
.network-links {
  display: grid;
  gap: var(--spacing-200);
}
</style>
