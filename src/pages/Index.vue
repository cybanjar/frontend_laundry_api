<template>
  <q-page class="flex flex-center">
    <img
      alt="Quasar logo"
      src="~assets/quasar-logo-full.svg"
    >
    
    <q-btn unelevated color="primary" label="Save" />
    <p>{{ name }}</p>
  </q-page>
</template>


<script>
import { reactive, toRefs, onMounted } from "@vue/composition-api";

export default {
  name: 'PageIndex',

  data() {
    return {
      name: 'Ahmad'
    }
  },

  mounted() {
    console.log('Mounted!');
  }

  // setup() {
  //   const state = reactive({
  //     name: 'Amin'
  //   });

  //   onMounted(() => {
  //     console.log('Mounted!');
  //   })

  //   return {
  //     ...toRefs(state),
  //   }
  // }
}
</script>
