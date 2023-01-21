<template>
  <div>
    <div class="skewed-header">
      <div class="header-bg" :style="bgImage"></div>
      <div class="skewed-header-wrapper"></div>
    </div>
    <!-- <profile-section class="profile-section" :profile="profile" /> -->
  </div>
</template>

<script>
// import ProfileSection from "@/components/ProfileSection.vue";
export default {
  name: "HeaderImage",
  components: {
    //  ProfileSection
  },
  props: {
    imageSrc: {
      type: String,
      required: true,
    },
    profile: {
      type: Object,
      required: true,
    },
  },
  computed: {
    bgImage() {
      return `background-image: url('images/background/${this.imageSrc}'`;
    },
  },
};
</script>
<style lang="scss" scoped>
.skewed-header {
  position: relative;
  height: 400px;
  overflow: hidden;
}
.skewed-header > .header-bg {
  position: absolute;
  top: 0;
  bottom: 0;
  right: 0;
  left: 0;
  height: 100%;
  width: 100%;
  background-repeat: no-repeat;
  background-size: cover;
  transform: skewY(-4deg);
  transform-origin: top left;
}
</style>
