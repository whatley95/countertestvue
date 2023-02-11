<template>
  <div class="app">
    <nav>
      <RouterLink to="/">C1</RouterLink> |
      <RouterLink to="/about">C2</RouterLink>
    </nav>

    <RouterView />
  </div>

</template>

<style>
.app {
  text-align: center;
}
</style>