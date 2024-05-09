<template>
  <div>
    hello world!{{count}}
    <button @click="count++">add</button>
    <Button></Button>
  </div>
</template>

<script lang="tsx">
import { Vue, Component } from 'vue-property-decorator';
import Button from './button.vue';

@Component({
  components: {
    Button
  }
})
export default class App extends Vue {
  count: number = 0;
}
</script>