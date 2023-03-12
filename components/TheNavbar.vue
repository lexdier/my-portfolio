<template>
  <BNavbar sticky class="">
    <BContainer>
      <BRow align-v="center" class="w-100">
        <BCol cols="7">
          <span>Logo</span>
        </BCol>
        <BCol cols="auto">
          <BNavbarNav>
            <BNavItem>Some</BNavItem>
            <BNavItem>Some</BNavItem>
            <BNavItem>Some</BNavItem>
          </BNavbarNav>
        </BCol>
      </BRow>
    </BContainer>
  </BNavbar>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator';

@Component({ components: {} })
export default class TheNavbar extends Vue {

}

</script>


