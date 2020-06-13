<template>
  <div>
    <TheHeader @sidenavToggle="displaySideNav = !displaySideNav" />
    <TheSidenav :show="displaySideNav" @close="displaySideNav = false" />
    <nuxt />
  </div>
</template>
<script>
import TheHeader from "~/components/Navigation/TheHeader";
import TheSidenav from "~/components/Navigation/TheSidenav";
export default {
  data() {
    return {
      displaySideNav: false
    };
  },
  components: {
    TheHeader,
    TheSidenav
  }
};
</script>

<style>
html {
  font-family: "Open Sans", sans-serif;
}
body {
  margin: 0;
  padding: 0;
}
</style>
