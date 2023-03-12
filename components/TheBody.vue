<template>
  <main>
    <section class="pb-5">
      <AnimationSection />
    </section>
    <section class="pb-5">
      <CardList />
    </section>
  </main>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator';
import AnimationSection from '~/components/AnimationSection.vue';
import CardList from '~/components/CardList.vue';

@Component({ components: { AnimationSection, CardList } })
export default class TheBody extends Vue {

}
</script>

