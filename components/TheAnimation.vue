<template>
  <div class="w-100 h-100">
    <div ref="animation" />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator';
import lottie from 'lottie-web';

@Component({})
export default class TheAnimation extends Vue {

  private animation: any;

  mounted() {
    this.animation = lottie.loadAnimation({
      container: this.$refs.animation as HTMLElement,
      renderer: 'svg',
      loop: true,
      autoplay: true,
      animationData: require('@/assets/animations/laptop_3.json'),
    });
  }

}
</script>
