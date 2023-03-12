<template>
  <BRow>
    <BCol v-for="item in listItems">
      <BCard :bg-variant="item.bgVariant" :title="item.title" text-variant="white">
        <b-card-text>
          Some quick example text to build on the <em>card title</em> and make up the bulk of the card's
          content.
        </b-card-text>

        <b-card-text>A second paragraph of text in the card.</b-card-text>

      </BCard>
    </BCol>
  </BRow>
</template>

<script lang="ts">
import { Component, Vue } from 'nuxt-property-decorator';

@Component({})
export default class CardList extends Vue {

  public listItems = [
    { title: 'Project', bgVariant: 'primary' },
    { title: 'Project-1', bgVariant: 'info' },
    { title: 'Project-2', bgVariant: 'success' },
    { title: 'Project-3', bgVariant: 'danger' },
  ];
}
</script>
