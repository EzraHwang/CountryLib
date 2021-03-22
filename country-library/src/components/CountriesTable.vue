<template>
   <table class="table">
    <thead>
    </thead>
    <tbody>
      <tr v-for="(item, key) in data" :key="key">
        <td>{{ item.name }}</td>
        <td>{{ item.cash }}</td>
        <td>{{ item.icash }}</td>
      </tr>
    </tbody>
  </table>
</template>