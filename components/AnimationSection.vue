<template>
  <BRow class="w-100" align-v="end">
    <BCol cols="6">
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
        </BCardBody>
        <div class="d-flex justify-content-around">
          <BBtn variant="outline-primary">
            <span>Something</span>
          </BBtn>
          <BBtn variant="outline-primary">
            <span>Something else</span>
          </BBtn>
        </div>
      </BCard>
    </BCol>
    <BCol cols="6">
      <TheAnimation />
    </BCol>
  </BRow>
</template>

<script lang="ts">

import { Component, Vue } from 'nuxt-property-decorator';
import TheAnimation from '~/components/TheAnimation.vue';

@Component({ components: { TheAnimation } })
export default class AnimationSection extends Vue {

}
</script>

