<template>
  <div id="app">
    <section-api></section-api>
  </div>
</template>

<script>

import SectionApi from './components/SectionApi.vue';

export default {
  name: 'App',
  components: {
    SectionApi,
  },
  data() {
    return{
      title: 'Vivo en vue',
    }
  }
}
</script>

