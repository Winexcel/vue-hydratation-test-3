<script>
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
  render(h) {
    debugger;
    console.log(this.$el);
    return h('div', [
        h('span', 'timestamp'),
        h('button', {
          on: {
            click: this.showMessage.bind(this),
          }
        }, 'Show Message')
    ]);
  }
}
</script>

<style scoped>

</style>