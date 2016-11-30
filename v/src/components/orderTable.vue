<template lang="html">
  <section class="order-table">
    <table>
      <thead>
        <th v-for="th of ths">
          {{ th }}
        </th>
      </thead>
      <tbody>
        <tr v-for="item of items">
          <td>{{ item.id }}</td>
          <td>{{ item.content }}</td>
        </tr>
      </tbody>
    </table>
  </section>
</template>

<script>
export default {
  name: 'OrderTable',
  props: ['ths', 'items']
}
</script>

<style lang="css">
</style>
