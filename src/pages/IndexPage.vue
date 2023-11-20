<template>
  <q-page class="flex flex-center">

  <div class="q-pa-md q-gutter-sm">

    <q-btn label="старт" size="xl" color="primary" @click="fullHeight = true" />

    <q-dialog
      v-model="fullHeight"
      full-height
    >
      <q-card class="column full-height" style="width: 300px">
        <q-card-section>
          <div class="text-h6">Введите</div>
        </q-card-section>

        <q-card-section class="col q-pt-none">
          input
        </q-card-section>
        <q-card-section class="col q-pt-none">
          input
        </q-card-section>
        <q-card-section class="col q-pt-none">
          input
        </q-card-section>
        <q-card-section class="col q-pt-none">
          input
        </q-card-section>
        <q-card-section class="col q-pt-none">
          input
        </q-card-section>


        <q-card-actions align="right" class="bg-white text-teal">
          <q-btn flat label="Далее" v-close-popup />
        </q-card-actions>
      </q-card>
    </q-dialog>
  </div>
  </q-page>
</template>

<script>
export default {
  name: "IndexPage",
  data() {
    return {
      isNone: false,
      fullHeight: false
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
