<template>
  <q-layout>
    <q-header>
      <q-toolbar>
        <q-toolbar-title>
          PopupTest
        </q-toolbar-title>
      </q-toolbar>
    </q-header>
    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
import { defineComponent, ref } from 'vue';

export default defineComponent({
  name: 'MainLayout',

  setup () {


    return {
        }
  }
})
</script>
