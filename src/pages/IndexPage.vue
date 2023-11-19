<template>
  <q-page class="flex flex-center">
    <div class="q-pa-md q-gutter-sm">
    <q-btn color="accent" class="btnStart"  @click="isNone = !isNone" :class="{btnNone: isNone}">
        Н а ч а т ь
    </q-btn>
  </div>
  </q-page>
</template>

<script>
export default {
  name: "IndexPage",
  data() {
    return {
      isNone: false,
    };
  },

  methods: {

  },
};
</script>

<style>
  .btnStart{
    height: 50px;
    width: 200px;
  }
  .btnNone{
    display: none;
  }
</style>
