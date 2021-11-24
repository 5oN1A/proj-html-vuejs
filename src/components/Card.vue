<template>
  <div class="col">
    <div class="card" style="width: 18rem">
      <img v-bind:src="require('@/assets/' + list.img)" />
      <div class="card-body">
        <h3 class="card-title">{{ list.title }}</h3>
        <p class="card-date">{{ list.date }}</p>
        <hr />
        <p class="card-text">{{ list.description }}</p>
      </div>
    </div>
  </div>
</template>


<script>
export default {
  name: "Card",
  props: {
    list: Object,
  },
  data() {
    return {};
  },
};
</script>