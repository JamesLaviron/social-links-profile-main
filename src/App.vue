<template>
  <main>
    <img
      src="../assets/images/avatar-sydney.jpeg"
      alt="article illustration"
      class="user-avatar"
    />
    <div class="user-info">
      <h1 class="user-name text-preset-1">Victor Gerfaud</h1>
      <h2 class="user-location text-preset-2-bold">
        Kremlin-Bicêtre, Val-de-Marne, France
      </h2>
    </div>
    <div class="user-bio text-preset-2">I feel like a turtle</div>
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
/* Main Mobile first */
main {
  display: grid;
  padding: var(--spacing-300);
  text-align: center;
  border-radius: 1.2rem;
  width: min-content;
  color: white;
  gap: var(--spacing-300);
  background-color: var(--color-grey-800);
}

/* Tablet */
@media screen and (min-width: 768px) {
  main {
    padding: var(--spacing-500);
    margin: var(--spacing-300) 0;
  }
}

/* Desktop */
@media screen and (min-width: 1440px) {
  main {
    padding: var(--spacing-500);
    margin: var(--spacing-300) 0;
  }
}

.user-avatar {
  width: 8.8rem;
  height: 8.8rem;
  border-radius: 99.9rem;
  margin: 0 auto;
}

.user-info {
  display: grid;
  min-width: 280px;
  gap: var(--spacing-50);
}
</style>
