<template>
  <putValue></putValue>
</template>

<script>
import putValue from '../components/putValue.vue'
export default {
  name: "IndexPage",
  components: {putValue},
  data() {
    return {
    };
  },

  methods: {
    isSecondDilogTrue(){
      this.isSecondDilog = true;
    }
  },
};
</script>

<style>

</style>
