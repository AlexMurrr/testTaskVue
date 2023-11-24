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
          <h5 class="hDialog">{{ item.label }}:</h5>
          <p class="pDialog">{{ item.value }}</p>
        </q-card-section>

        <q-card-actions align="right" class="bg-white text-teal">
          <q-btn flat label="Ok" v-close-popup @click="toFalseVisibleDialod"/>
        </q-card-actions>
      </q-card>
    </q-dialog>
  </div>
</template>

<script>

export default {
  name: "inputValue",
  props: {
    items: {
      type: Array,
      default: [{label: 'Ваших данных нет', value: ''},],
      required: true,
      }
    },
  data() {
    return {
      fullHeight:true,
      };
    },

    methods: {
      toFalseVisibleDialod() {
      this.$emit('toFalse', false);
      }
    },
  }

</script>

<style>
.hDialog{
  margin: 14px;
}

.pDialog{
  font-size: 22px;
}
</style>
