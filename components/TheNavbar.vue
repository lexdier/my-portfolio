<template>
  <BNavbar sticky style="background-color: whitesmoke">
    <BContainer>
      <BRow align-v="center" class="w-100">
        <BCol cols="7">
          <BImg width="70" src="https://cdn-icons-png.flaticon.com/512/57/57062.png" alt="" />
        </BCol>
        <BCol cols="5">
          <BNavbarNav>
            <BNavItem>
              <span class="text-dark text-uppercase">
                Some
              </span>
            </BNavItem>
            <BNavItem>
              <span class="text-dark text-uppercase">
                Some
              </span>
            </BNavItem>
            <BNavItem>
              <span class="text-dark text-uppercase">
                Some
              </span>
            </BNavItem>
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


