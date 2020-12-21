<template>
  <component :is="blok.component" v-bind="blok" :blok="blok"></component>
</template>

<script>
export default {
  inheritAttrs: false,
  props: {
    blok: Object
  }
};
</script>
