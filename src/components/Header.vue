<template>
  <header>
    <div
      class="container-fluid d-flex align-items-center justify-content-between"
    >
      <img class="logo" src="../assets/construction_logo.png" alt="" />
      <nav class="pt-4">
        <ul class="d-flex align-items-center">
          <li
            v-for="(item, i) in navItems"
            :key="i"
            :class="i === currentActive ? 'active' : ''"
          >
            <a :href="item.href">{{ item.title }}</a>
          </li>
          <a class="my_btn my_btn_yellow" href="#">GET QUOTE</a>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
  components: {},
  data() {
    return {
      navItems: [
        {
          title: "HOME",
          href: "#",
        },
        {
          title: "ABOUT",
          href: "#",
        },
        {
          title: "SERVICES",
          href: "#",
        },
        {
          title: "WORK",
          href: "#",
        },
        {
          title: "ARTICLES",
          href: "#",
        },
      ],
      currentActive: 0,
    };
  },
  computed: {},
  methods: {},
  mounted() {},
};
</script>