<template>
  <nav>
    <ul>
      <li>
        <NuxtLink to="/learn/structural">Structural </NuxtLink>
      </li>
      <li>
        <NuxtLink to="/learn/other1">Data handling</NuxtLink>
      </li>
      <li>
        <NuxtLink to="/learn/other2">Other 2</NuxtLink>
      </li>
      <li>
        <NuxtLink to="/learn/other3">Other 3</NuxtLink>
      </li>
      <li>other 4</li>
    </ul>
  </nav>
</template>

<style scoped>
nav {
  grid-area: nav;
  margin-right: 5rem;
  height: 90vh;
}
</style>
