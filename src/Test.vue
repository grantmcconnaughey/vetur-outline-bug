<template>
  <div>
    {{ test }}
  </div>
</template>

<script>
export default {
  props: ['foo', 'bar'],
  data() {
    return {
      test: 'hello'
    }
  },
  computed: {
    test2() {
      return this.test
    }
  },
  mounted () {
    console.log('mounted');
  },
}
</script>