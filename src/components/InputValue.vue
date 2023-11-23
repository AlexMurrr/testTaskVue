<template>
  <div>
    <q-dialog
      v-model="fullHeight"
      full-height
    >
      <q-card class="column full-height" style="width: 300px">
        <q-card-section>
          <div class="text-h6"></div>
        </q-card-section>

        <q-card-section v-for="item in items" class="col q-pt-none">
          <q-input :label=item.label v-model=item.value />
        </q-card-section>

        <q-card-actions align="right" class="bg-white text-teal">
          <q-btn flat label="Далее" v-close-popup />
        </q-card-actions>
      </q-card>
    </q-dialog>
  </div>
</template>

<script>
export default {
  name: "InputValue",
  props: {
    isSecondDilog: {
            type:Boolean
        }

    },
  data() {
    return {
      fullHeight: this.isSecondDilog,
      }
    }
  }
</script>

<style>


</style>
