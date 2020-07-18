<template>
  <div class="about">
    <h1>This is an about page</h1>
    <AboutMe :name="myName" :age="myAge" />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import AboutMe from '@/components/AboutMe.vue';

@Component({
  components: {
    AboutMe,
  },
})
export default class About extends Vue {
  private myName: string = 'David';
  private myAge: number = 101;
}
</script>
