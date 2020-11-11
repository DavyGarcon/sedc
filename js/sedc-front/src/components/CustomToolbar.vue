<template>
  <md-toolbar class="md-transparent md-absolute md-layout" md-elevation="0">
    <div class="md-layout-item md-size-20">
      <img
        :id="logo"
        :src="logo"
        alt="Saint Etienne de Chigny"
        class="rounded-circle"
        :class="{ 'responsive-image': responsive }"
      />
    </div>
    <div class="md-layout-item md-size-80">
      <custom-menu></custom-menu>
    </div>
  </md-toolbar>
</template>

<script>
import CustomMenu from "@/components/CustomMenu";

export default {
  name: "custom-toolbar",
  components: { CustomMenu },
  data: () => {
    return {
      logo: require("@/assets/img/faces/avatar.jpg"),
      responsive: true
    };
  },
  methods: {}
};
</script>