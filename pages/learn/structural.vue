<template>
  <NuxtLayout name="learning">
    <div>
      <h2>Structural Stuff</h2>
      <h3>Only one Root Element in Pages</h3>
      <p>
        Pages should not have more than 1 root element and must not start with a
        comment to make them work properly with client side navigation regarding
        the Nuxt Docs. But in the example below both work.
      </p>
      <div class="example">
        <p>
          This is an example with a <strong>nested view</strong>, i.e. a Nuxt
          Child Page:
        </p>

        <button>
          <NuxtLink to="/learn/structural/example-multiple-root-components"
            >Routing can break here
          </NuxtLink>
        </button>

        <button>
          <NuxtLink
            noPrefetch
            to="/learn/structural/example-single-root-component"
            >Routing should work
          </NuxtLink>
        </button>
        <div class="childPage">
          <NuxtPage page-key="example" />
        </div>
      </div>
      <h3>Nested Components</h3>
      <p>
        Components can be organized in nested folders. Auto import should still
        work. The components need to have the folder names as an prefix.
        Duplicated Names in the structure are removed.
      </p>
      <p>
        Example: <br />
        /Overview/Header/Header.vue => &lt; OverviewHeader /> <br />
        /Overview/Header/Search.vue => &lt; OverviewHeaderSearch />
      </p>
    </div>
  </NuxtLayout>
</template>

<script setup lang="ts"></script>

<style scoped>
.example {
  padding: 1rem;
  border: solid 2px;
}
.childPage {
  margin-top: 1rem;
  padding: 0.5rem 1rem;
  background: lightgrey;
}
</style>
