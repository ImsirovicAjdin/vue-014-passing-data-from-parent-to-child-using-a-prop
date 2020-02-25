<template>
  <div id="app">
    <HelloWorld v-bind:content="datacontent" />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld";

export default {
  name: "App",
  components: {
    HelloWorld
  },
  data() {
    return {
      datacontent: `This parent data (i.e the 'datacontent') was bound to a prop
          of the child component and thus made available inside the child
          component itself`
    }
  }  
};
</script>

