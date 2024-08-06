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
export default {
  name: "NetworkLinksList",
  props: {
    msg: String,
  },
};
</script>

<style scoped>
.network-links {
  display: grid;
  gap: var(--spacing-200);
}
</style>
