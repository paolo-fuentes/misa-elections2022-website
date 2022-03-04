<template>
  <div id="app">
    <router-view name="header" v-if="!['Elections', 'Ballot', 'invalidID'].includes($route.name)" />
    <div class="wrapper">
      <router-view />
    </div>
    <router-view name="footer" v-if="!['Elections', 'Ballot', 'invalidID'].includes($route.name)" />
  </div>
</template>
<script>
export default {};
</script>
