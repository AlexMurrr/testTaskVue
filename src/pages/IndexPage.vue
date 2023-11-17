<template>
  <q-page class="flex flex-center">
    <div class="q-pa-md q-gutter-sm">
    <q-btn color="primary" class="btnStart">
        Н а ч а т ь
    </q-btn>
  </div>
  </q-page>
</template>

<script>
import { defineComponent } from 'vue'
//import buttonStart from "../components/btnQ.vue";

export default defineComponent({
  name: 'IndexPage'
})
</script>

<style>
  .btnStart{
    display: inline;
    height: 50px;
    width: 200px;
  }
</style>
