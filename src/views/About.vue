<template>
  <div class="about">
    <h1>This is an about page</h1>
    <AboutMe :name="myName" :age="myAge" :phrase="myPhrase"/>
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
  private myName: string = 'Seulki Bae';
  private myAge: number = 3;
  private myPhrase: string = 'I\'m hungry';
}
</script>
