<template>
  <q-page class="flex flex-center">
    <img
      alt="Quasar logo"
      src="~assets/quasar-logo-full.svg"
    >
    
    <q-btn unelevated color="primary" @click="onClick" label="Save" />
    <!-- <p>{{ name }}</p> -->
  </q-page>
</template>


<script>
import { reactive, toRefs, onMounted } from "@vue/composition-api";

export default {
  name: 'PageIndex',

  setup() {
    const state = reactive({
      name: 'Ahmad'
    });

    onMounted(() => {
      console.log('Mounted!');
    });

    const onClick = () => {
      console.log("ok");
    }

    return {
      ...toRefs(state),
      onClick
    }
  }
}
</script>
