<template>
  <div class="home">
    <BigTitle left-message="<" left-message-color="Hello " right-message-color="Waffel" right-message="/>"/>
  </div>
</template>

<script lang="ts">
  import { Component, Vue } from 'vue-property-decorator';
  import BigTitle from '@/components/BigTitle.vue';

  @Component({
    components: {
     BigTitle,
    },
  })
  export default class Home extends Vue {}
</script>
