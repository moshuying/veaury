<template>
  <h3>
    This example shows the basic usage of `applyReactInVue`.
  </h3>
  <h4>
    Using React components in Vue components.
  </h4>
  <AA />
</template>

<script>
import { onMounted, onUnmounted, ref, getCurrentInstance, nextTick } from 'vue'
import { applyPureReactInVue, applyReactInVue } from 'veaury'
// This is a React Component
// import ReactBasic from "./react_app/Basic"
import ReactAA from "./react_app/App"
// import ReactBB from "./react_app/BB"
// import ReactCC from "./react_app/CC"

export default {
  components: {
    // Basic: applyReactInVue(ReactBasic),
    AA: applyReactInVue(ReactAA),
    // BB: applyReactInVue(ReactBB),
    // CC: applyReactInVue(ReactCC)
  },
  setup() {
    return
  }
}
</script>

<style scoped>
.slot {
  background: aquamarine;
  padding: 10px;
  margin: 10px;
}
</style>
