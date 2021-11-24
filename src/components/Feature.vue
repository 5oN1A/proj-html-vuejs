<template>
  <div class="col">
    <div class="block p-3">
      <div class="icon_wrapper text-center pb-3">
        <i class="fa" :class="list.icon" aria-hidden="true"></i>
      </div>
      <h2>{{ list.title }}</h2>
      <p>{{ list.description }}</p>
      <div class="overlay p-3">
        <h6 class="pt-3">ARTFULLY CRAFTED</h6>
        <p class="pt-1">
          Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam
          nihil molestiae consequatur, vel illum qui dolorem eum.
        </p>
        <a class="my_btn">GET A QUOTE</a>
      </div>
    </div>
  </div>
</template>


<script>
export default {
  name: "Feature",
  props: {
    list: Object,
  },
  data() {
    return {};
  },
};
</script>
