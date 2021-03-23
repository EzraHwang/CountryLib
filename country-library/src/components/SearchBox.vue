<template>
  <b-input-group class="mt-3" size="lg">
    <b-form-input v-model="text" placeholder="Enter Country Name / Code to search" type=search></b-form-input>
    <b-input-group-append>
      <b-button variant="info">GO!</b-button>
    </b-input-group-append>
  </b-input-group>
</template>

<script>
export default {
  data() {
    return {
      text: "",
    };
  },
};
</script>