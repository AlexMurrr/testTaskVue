<template>
  <div>

  </div>
</template>

<script>
export default {
  name: "InputValue",
  data() {
    return {
      isNone: false,
      fullHeight: false,
      items:[{label: 'Фамилия', value: ''},
             {label:'Имя', value:''},
             {label:'Отчество', value:''},
             {label:'Специальность', value:''},
             {label:'Опыт', value:''},]
    };
   }
  }
</script>
