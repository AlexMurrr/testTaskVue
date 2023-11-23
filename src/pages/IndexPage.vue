<template>
  <q-page class="flex flex-center">

  <div class="q-pa-md q-gutter-sm">

    <q-btn label="старт" size="xl" color="primary" @click="isSecondDilogTrue()" />

    <q-dialog
      v-model="fullHeight"
      full-height
    >
      <q-card class="column full-height" style="width: 300px">
        <q-card-section>
          <div class="text-h6">Введите:</div>
        </q-card-section>

        <q-card-section v-for="item in items" class="col q-pt-none">
          <q-input :label=item.label v-model=item.value />
        </q-card-section>

        <q-card-actions align="right" class="bg-white text-teal">
          <q-btn flat label="Далее" v-close-popup @click="isSecondDilogTrue()"/>
        </q-card-actions>
      </q-card>
    </q-dialog>
  </div>
  <InputValue :isSecondDilog=isSecondDilog></InputValue>
  </q-page>
</template>

<script>
import InputValue from '../components/InputValue.vue'
export default {
  name: "IndexPage",
  components: {InputValue},
  data() {
    return {
      isSecondDilog : false,
      fullHeight: false,
      items:[{label: 'Фамилия', value: ''},
             {label:'Имя', value:''},
             {label:'Отчество', value:''},
             {label:'Специальность', value:''},
             {label:'Опыт', value:''},]
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
