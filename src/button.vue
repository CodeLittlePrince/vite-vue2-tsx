<script lang="tsx">
import { Vue, Component } from 'vue-property-decorator';

@Component
export default class Button extends Vue {
  message: string = 'Hello, Vue!';

  onClick() {
    this.message = 'Hello, World!'
  }

  render() {
    return (
      <button onClick={this.onClick}>
        {this.message}
      </button>
    )
  }
}
</script>