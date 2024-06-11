<template>
  <div class="card">
    <div id="title"><strong>Page Title</strong></div>
    <OverviewContentGridPageCardBreadcrumbs id="breadcrumbs" />
    <OverviewContentGridPageCardVersionPreview />
  </div>
</template>

<style scoped>
.card {
  display: flex;
  flex-direction: column;
  width: 200px;
  padding: 10px;
  background: beige;
}

#title {
  grid-template-areas: title;
}

#breadcrumbs {
  grid-template-areas: breadcrumbs;
}
</style>
