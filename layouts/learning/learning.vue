<template>
  <div class="root-container">
    <h1 id="heading">Nuxt Learning Info:</h1>
    <button>
      <NuxtLink to="/"> return to App </NuxtLink>
    </button>
    <LearningNavigation />
    <div>
      <slot />
    </div>
  </div>
</template>

<style scoped>
.root-container {
  display: grid;
  grid-template:
    'heading heading link'
    'nav content content';
}
#heading {
  grid-area: heading;
}
nav {
  grid-area: nav;
  margin-right: 5rem;
  height: 90vh;
}
button {
  font-size: 1.3rem;
}
</style>
