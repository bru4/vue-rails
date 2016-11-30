<template lang="html">
  <section class="index">
    <OrderTable v-bind:ths="ths" v-bind:items="items"></OrderTable>
  </section>
</template>

<script>
import OrderTable from '../components/orderTable'

export default {
  name: 'Index',
  components: {
    OrderTable
  },
  data() {
    return {
      ths: ['a', 'b', 'c', 'd'],
      items: [
        { id: '1', content: '111' }
      ]
    }
  }
}
</script>

<style lang="css">
</style>
