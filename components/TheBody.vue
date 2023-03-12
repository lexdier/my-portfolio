<template>
  <BRow class="w-100">
    <BCol cols="6" align-self="end">
      <BCard class="border-0">
        <BCardTitle>
          <span>New way to Build your Dreams</span>
        </BCardTitle>
        <BCardBody>
          <p>
            Meet Dexam Highly customizable Pure Vue JS + Bootstrap 4 Landing
            Pages.
          </p>
          <div class="mb-5 lead">
            <ul class="list-inline">
              <li class=" mb-3 ">
                <span>Minimal, Intuitive and Fully Responsive Design</span>
              </li>
              <li class="mb-3"><i class="eva eva-checkmark-outline mr-2 text-warning"></i>
                Super Flexible And Customizable
              </li>
            </ul>
          </div>
          <div>
            <BBtn variant="outline-primary">
              <span>Something</span>
            </BBtn>
            <BBtn variant="outline-primary">
              <span>Something else</span>
            </BBtn>
          </div>
        </BCardBody>
      </BCard>
    </BCol>
    <BCol cols="6">
      <div class="w-100 h-100">
        <div ref="animation" />
      </div>
    </BCol>
  </BRow>
</template>


<script lang="ts">
import lottie from 'lottie-web';
import { Component, Vue } from 'nuxt-property-decorator';

@Component({ components: {} })
export default class TheBody extends Vue {

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

