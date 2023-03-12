<template>
  <BContainer>
    <section>
      <TheBody />
    </section>
  </BContainer>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator';
import TheBody from '@/components/TheBody.vue';

@Component({ components: { TheBody } })
export default class IndexPage extends Vue {

}
</script>
