<template>
  <div class="about-me">
    <h2>Hello everyone, my name is {{ name }}.</h2>
    <h3>I'm {{ age }}</h3>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class AboutMe extends Vue {
  @Prop() private name!: string;
  @Prop() private age!: number;
}
</script>
