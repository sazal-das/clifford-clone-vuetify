<template>
  <div :style="dark ? 'background-color: #242424' : 'background-color:#F4F4F7;'">
    <header-image :image-src="'background2.jpg'" :profile="profileInfo" />
    <profile-section :profile="profileInfo" :dark="dark" :solo="true" />
    <div class="pb-10" style="max-width: 1000px; margin: 0 auto;">
      <div>
        <div class="mt-5" style="width: 80%; margin: 0 auto;">
          <item-card :item="firstItem" :dark="dark" />
        </div>
        <div class="mt-5" style="width: 80%; margin: 0 auto;">
          <iframe
            style="width: 100%; margin: 0 auto;"
            title="vimeo-player"
            src="https://www.youtube.com/embed/pyOi4bW4QRg"
            width="640"
            height="360"
            frameborder="0"
            allowfullscreen
          ></iframe>
        </div>
        <div class="mt-5" style="width: 80%; margin: 0 auto;">
          <v-row>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
          </v-row>
        </div>
      </div>
      <!-- Phone Customization -->
      <div>
        <div class="text-h6 mt-10 font-weight-bold grey-text text-center">Phone Customization</div>
        <div class="mt-5" style="width: 80%; margin: 0 auto;">
          <v-row>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
          </v-row>
        </div>
      </div>
      <!-- Camera Gear -->
      <div>
        <div class="text-h6 mt-10 font-weight-bold grey-text text-center">Camera Gear</div>
        <div class="mt-5" style="width: 80%; margin: 0 auto;">
          <v-row>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
          </v-row>
        </div>
      </div>
      <!-- Desk Setup -->
      <div>
        <div class="text-h6 mt-10 font-weight-bold grey-text text-center">Desk Setup</div>
        <div class="mt-5" style="width: 80%; margin: 0 auto;">
          <v-row>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
          </v-row>
        </div>
      </div>
      <!-- Desk Peripherals -->
      <div>
        <div class="text-h6 mt-10 font-weight-bold grey-text text-center">Desk Peripherals</div>
        <div class="mt-5" style="width: 80%; margin: 0 auto;">
          <v-row>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
          </v-row>
        </div>
      </div>
      <!-- PC Parts -->
      <div>
        <div class="text-h6 mt-10 font-weight-bold grey-text text-center">PC Parts</div>
        <div class="mt-5" style="width: 80%; margin: 0 auto;">
          <v-row>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
          </v-row>
        </div>
      </div>
      <!-- Lighting -->
      <div>
        <div class="text-h6 mt-10 font-weight-bold grey-text text-center">Lighting</div>
        <div class="mt-5" style="width: 80%; margin: 0 auto;">
          <v-row>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
          </v-row>
        </div>
      </div>
      <hr class="my-5" style="max-width: 800px; margin: 0 auto;" />
      <div>
        <div class="mt-5" style="width: 80%; margin: 0 auto;">
          <item-card :item="firstItem" :dark="dark" />
        </div>
        <div class="mt-5" style="width: 80%; margin: 0 auto;">
          <v-row>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="firstItem" :dark="dark" />
            </v-col>
          </v-row>
        </div>
      </div>
    </div>
    <div style="width: max-content; margin: 0 auto;cursor: pointer;" class="pb-10 d-flex">
      <v-img src="solo-icon.svg" width="40"></v-img>
      <div class="ml-3 footer-text">create your own page</div>
    </div>
  </div>
</template>

<script>
import HeaderImage from "@/components/HeaderImage.vue";
import ProfileSection from "@/components/ProfileSection.vue";
import ItemCard from "@/components/ItemCard.vue";
export default {
  name: "SoloView",
  components: {
    HeaderImage,
    ProfileSection,
    ItemCard,
  },
  data() {
    return {
      dark: true,
      profileInfo: {
        imageSrc: "profile2.jpg",
        name: "Shevon Salmon",
        address: "Toronto",
        info: "• Tech • Lifestyle • Good Vibes ✨",
      },
      firstItem: {
        image: "solo/item1.jpg",
        name: "Melgeek Pixel Keyboard",
        description: "bit.ly/3sy1Hlw",
      },
    };
  },
};
</script>
<style lang="scss" scoped>
.grey-text {
  color: #51534a;
}
.footer-text {
  color: #848484;
}
.footer-text:hover {
  color: white;
}
</style>
