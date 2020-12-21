<template>
  <div>
    <h2>Container</h2>
    <DynamicComponent
      v-for="blok in body"
      :key="blok.id"
      :blok="blok"
      class="child"
      style="border: 1px solid black"
    />
  </div>
</template>

<script>
export default {
  inheritAttrs: false,
  props: {
    body: Array
  }
};
</script>
<style>
.child {
  background-color: red;
}
</style>
