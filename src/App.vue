<template>
  <div class="outer-shell">
    <Header></Header>
    <Main
      :features="featuresList"
      :qualities="qualitiesList"
      :news="newsList"
    ></Main>
    <Footer></Footer>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Main from "@/components/Main.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer,
  },
  data() {
    return {
      featuresList: [
        {
          icon: "fa-building",
          title: "Buildings",
          description:
            "Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur.",
        },
        {
          icon: "fa-refresh",
          title: "Renovate",
          description:
            "Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur.",
        },
        {
          icon: "fa-home",
          title: "Construct",
          description:
            "Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur.",
        },
        {
          icon: "fa-truck",
          title: "Exclusive",
          description:
            "Quis autem vel eum iure reprederit qui in ea voluptate velit esse quam nihil molestiae consequatur.",
        },
      ],
      qualitiesList: [
        {
          icon: "fa-home",
          title: "Great Services",
          description:
            "Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia",
        },
        {
          icon: "fa-cog",
          title: "Highest Standards",
          description:
            "Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia",
        },
        {
          icon: "fa-users",
          title: "Professional Team",
          description:
            "Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia",
        },
        {
          icon: "fa-lightbulb-o",
          title: "Creative Solutions",
          description:
            "Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia",
        },
      ],
      newsList: [
        {
          img: "blog-post-134132600-400x241.jpg",
          title: "Redeveloping Florida’s Remote Southern Coast",
          date: "December 7th, 2015",
          description:
            "Technology is Here to Stay Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus purus nisl, elementum vitae consequat at, tristique ut enim. Sed ut dignissim leo. Nullam sed metus id sapien faucibus rhoncus sed",
        },
        {
          img: "blog-post-92486644-400x241.jpg",
          title: "How We Manage Large Construction Projects",
          date: "December 7th, 2015",
          description:
            "Technology is Here to Stay Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus purus nisl, elementum vitae consequat at, tristique ut enim. Sed ut dignissim leo. Nullam sed metus id sapien faucibus rhoncus sed",
        },
        {
          img: "blog-post-332773904-400x241.jpg",
          title: "Future proofing a modern home",
          date: "December 6th, 2015",
          description:
            "Technology is Here to Stay Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus purus nisl, elementum vitae consequat at, tristique ut enim. Sed ut dignissim leo. Nullam sed metus id sapien faucibus rhoncus sed",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap";
@import "~font-awesome/css/font-awesome.css";
@import "styles/variables";
@import "styles/header";
@import "styles/main";
@import "styles/footer";
@import "styles/utilities";
</style>
