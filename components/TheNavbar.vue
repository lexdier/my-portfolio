<template>
  <BNavbar class="rounded">
    <BRow align-v="center w-100">
      <BCol lg="4">
        <BImg
          fluid
          width="100"
          src="data:image/png;base64,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" />
      </BCol>
      <BCol lg="4">
        <BNavbarNav class="d-flex justify-content-around">
          <BNavItem v-b-hover="handleAboutHover" :class="aboutIsHovered ? 'border-bottom ':'' ">About</BNavItem>
          <BNavItem v-b-hover="handleStudiesHover" :class="StudiesIsHovered ? 'border-bottom ':'' ">Studies</BNavItem>
          <BNavItem v-b-hover="handleContactHover" :class="ContactIsHovered ? 'border-bottom ':'' ">Contact</BNavItem>
        </BNavbarNav>
      </BCol>
      <BCol lg="4" class="d-flex justify-content-end">
        <span>Something else</span>
      </BCol>
    </BRow>
  </BNavbar>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator';

@Component({})
export default class TheNavbar extends Vue {
  public aboutIsHovered: boolean = false;
  public StudiesIsHovered: boolean = false;
  public ContactIsHovered: boolean = false;

  public handleAboutHover(hovered: any) {
    this.aboutIsHovered = hovered;
  }

  public handleStudiesHover(hovered: any) {
    this.StudiesIsHovered = hovered;
  }

  public handleContactHover(hovered: any) {
    this.ContactIsHovered = hovered;
  }
}
</script>


