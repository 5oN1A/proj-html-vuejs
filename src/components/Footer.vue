<template>
  <footer>
    <div class="container-fluid">
      <div class="row row-cols-4 g-5">
        <div class="col">
          <div>
            <img
              class="logo mb-4"
              src="../assets/construction_logo.png"
              alt="logo"
            />
            <p class="text-start pb-2">
              We are specialists in the construction of unique and exclusive
              properties. Our work inspires. We pride ourselves on delivering
              outstanding quality and design for leading clients across the
              world.
            </p>

            <a href="#" class="my_btn my_btn_yellow">LEARN MORE</a>
          </div>
        </div>
        <div class="col">
          <h5>LATEST TWEETS</h5>
          <div class="d-flex">
            <img
              class="theme_fusion"
              src="../assets/3a74ce3d0532b7773b174c45ca3bd05a_bigger.png"
              alt=""
            />
            <div class="ps-1 pb-3">
              <p class="m-0 p-0 lh-1 white-txt"><b>ThemeFusion</b></p>
              <p class="m-0 p-0 lh-1 white-txt"><i>@Theme_Fusion</i></p>
              <p class="m-0 pt-1 pb-3 lh-1 white-txt">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. dolor
                sit amet consectetur adipisicing elit.Repellendus repudiandae
                libero sequi eum maiores ipsum ex dolore excepturi quas non
                minus quia iure debitis, totam saepe, inventore beatae dicta
                odio!
              </p>
              <img
                class="discount"
                src="../assets/discount.png"
                alt="discount"
              />
            </div>
          </div>
        </div>
        <div class="col">
          <h5>CONTACT US TODAY</h5>
          <ul>


            <li v-for="(contact, i) in contactsList" :key="i" class="d-flex">
              <i class="fa lh-base " :class="contact.icon" aria-hidden="true"></i>
              <div class="ms-2 mb-2">
              <p>{{contact.description}}</p>
              <p v-if="contact.address">{{contact.address}}</p>
              <p v-if="contact.city">{{contact.city}}</p>
              </div>
            </li>




          </ul>
        </div>
        <div class="col">
          <h5>FIND US</h5>
          <img src="../assets/map.png" alt="map" />
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
  components: {},
  data() {
    return {
      contactsList: [
        {
          icon: "fa-globe",
          description: "Corporate Location",
          address: "1600 Amphitheatre Parkway",
          city:"London WC1 1BA"
          
        },
        {
          icon: "fa-home",
          description: "Residential Location",
          address:"9521 Broadsberry Avenue",
          city:"Paddington RC7 9ZA"
        },
        {
          icon: "fa-phone",
          description: "1.800.458.556 / 1.800.532.2112"
        },
        {
          icon: "fa-phone",
          description: "info@your-domain.com"
        },
        {
          icon: "fa-clock-o",
          description: "Monday – Friday: 9:00 AM – 6:00 PM"
        },
        {
          icon: "fa-clock-o",
          description: "Saturday – Sunday: 9:00 AM – 12:00 PM"
        },

      ],
    };
  },
  computed: {},
  methods: {},
  mounted() {},
};
</script>