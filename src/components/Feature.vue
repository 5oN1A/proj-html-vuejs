<template>
     <div class="col">
            <div class="block p-3">
              <div class="icon_wrapper text-center pb-3">
                <i class="fa" :class="list.icon" aria-hidden="true"></i>
              </div>
              <h2>{{list.title}}</h2>
              <p>{{list.description}}
              </p>
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
  }
};

</script>
