<script>
import {h} from 'vue';

export default {
  name: 'CurrentTimestamp',
  data() {
    return {
      time: Date.now(),
    }
  },
  mounted() {
    console.log(`Component: ${this.$options.name} mounted.`);
  },
  methods: {
    showMessage() {
      alert('Hello winni!');
    }
  },
  render() {
    debugger;
    console.log(this.$el);
    return h('div', [
        h('span', 'timestamp'),
        h('button', {
          onClick: this.showMessage.bind(this),
          }, 'Show Message')
    ]);
  }
}
</script>

<style scoped>

</style>