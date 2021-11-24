<template>
  <div class="col">
    <div class="quality is-active">
      <i class="fa circle-icon" :class="list.icon" aria-hidden="true"></i>
      <h6 class="pt-2 mb-0">{{ list.title }}</h6>
      <hr class="mb-1" />
      <p>{{ list.description }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Quality",
  props: {
    list: Object,
  },
  data() {
    return {};
  },
};
</script>
<style lang="scss">

</style>