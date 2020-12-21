<template>
  <div>
    <h1>Class / Style binding with dynamic components</h1>
    <DynamicComponent
      v-for="blok in body"
      :key="blok.id"
      :blok="blok"
      class="block"
    />
  </div>
</template>

<script>
export default {
  data: () => ({
    body: [
      {
        component: "ContainerComponent",
        id: 1,
        body: [
          { id: 2, title: "Child 1", component: "SimpleComponent" },
          { id: 3, title: "Child 2", component: "SimpleComponent" }
        ]
      }
    ]
  })
};
</script>

<style>
.block {
  background-color: blue;
}
</style>
