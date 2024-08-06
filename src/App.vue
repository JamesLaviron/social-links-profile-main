<template>
  <main>
    <img
      src="../assets/images/illustration-article.svg"
      alt="article illustration"
      class="user-avatar"
    />
    <div class="user-info">
      <h1 class="user-name text-preset-1">Victor Gerfaud</h1>
      <p class="user-location text-preset-2-bold">
        Kremlin-Bicêtre, Val-de-Marne, France
      </p>
    </div>
    <div class="user-bio text-preset-2"></div>
    <NetworkLinksList />
  </main>
</template>

<script>
import NetworkLinksList from "./components/NetworkLinksList.vue";

export default {
  name: "App",
  components: {
    NetworkLinksList,
  },
};
</script>

<style>
/* Mobile first */
main {
  display: grid;
  gap: 1rem;
  text-align: center;
  border-radius: 1.2rem;
  width: min-content;
  color: white;
  gap: var(--spacing-300);
  padding: var(--spacing-300);
}

/* Tablet */
@media screen and (min-width: 768px) {
  main {
    padding: var(--spacing-500);
    gap: var(--spacing-300);
  }
}

/* Desktop */
@media screen and (min-width: 1440px) {
  main {
    padding: var(--spacing-500);
    gap: var(--spacing-300);
  }
}

.user-avatar {
  width: 8.8rem;
  height: 8.8rem;
  border-radius: 99.9rem;
}
</style>
