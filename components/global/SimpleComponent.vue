<template>
  <div class="simple">Simple {{ title }}</div>
</template>

<script>
export default {
  inheritAttrs: false,
  props: {
    title: String
  }
};
</script>
