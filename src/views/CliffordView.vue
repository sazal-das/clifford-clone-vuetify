<template>
  <div style="background-color:#F4F4F7;">
    <header-image :image-src="'background1.jpg'" :profile="profileInfo" />
    <profile-section :profile="profileInfo" />
    <join-club />
    <div class="pb-10" style="max-width: 1000px; margin: 0 auto;">
      <!-- Online Store -->
      <div>
        <div class="text-h6 font-weight-bold grey-text text-center">ONLINE STORE</div>
        <div class="mt-5" style="width: 80%; margin: 0 auto;">
          <item-card :item="discountItem" />
        </div>
        <div class="mt-5" style="width: 80%; margin: 0 auto;">
          <v-row>
            <v-col cols="12" lg="6">
              <item-card :item="onlineItems[0]" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="onlineItems[1]" />
            </v-col>
          </v-row>
        </div>
      </div>
      <!-- Clifford Store -->
      <div>
        <div class="text-h6 mt-10 font-weight-bold grey-text text-center">CLIFFORD LUU</div>
        <div class="mt-5" style="width: 80%; margin: 0 auto;">
          <v-row>
            <v-col cols="12" lg="6">
              <item-card :item="cliffordItems[0]" />
            </v-col>
            <v-col cols="12" lg="6">
              <item-card :item="cliffordItems[1]" />
            </v-col>
          </v-row>
        </div>
      </div>
      <!-- Media -->
      <div>
        <div class="text-h6 mt-10 font-weight-bold grey-text text-center">MEDIA</div>
        <div class="mt-5" style="width: 80%; margin: 0 auto;">
          <iframe
            style="width: 100%; margin: 0 auto;"
            title="vimeo-player"
            src="https://player.vimeo.com/video/575163937?h=b8ba8632f1"
            width="640"
            height="360"
            frameborder="0"
            allowfullscreen
          ></iframe>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import HeaderImage from "@/components/HeaderImage.vue";
import ProfileSection from "@/components/ProfileSection.vue";
import JoinClub from "@/components/JoinClub.vue";
import ItemCard from "@/components/ItemCard.vue";
export default {
  name: "CliffordView",
  components: {
    HeaderImage,
    ProfileSection,
    JoinClub,
    ItemCard,
  },
  data() {
    return {
      profileInfo: {
        imageSrc: "profile1.jpg",
        name: "CLIFFORD LUU",
        address: "SYDNEY AUSTRALIA",
        info: "CAKER, BAKER + MAKER",
      },
      discountItem: {
        image: "item1.jpg",
        name: "COLOUR MILL",
        description: "10% Discount Code ( automatic link )",
      },
      onlineItems: [
        {
          image: "item2.jpg",
          name: "ONLINE COURSES",
          description: "Cakes by Cliff online courses",
        },
        {
          image: "item3.jpg",
          name: "THE WARD BROS APPAREL",
          description: "Hoodies & Sweaters ft Frenchies",
        },
      ],
      cliffordItems: [
        {
          image: "item4.jpg",
          name: "ABOUT CLIFFORD",
          description: "Find out more about me",
        },
        {
          image: "item5.jpg",
          name: "CAKE & BAKE RECIPES",
          description: "Cake decorating recipes",
        },
      ],
    };
  },
};
</script>
<style lang="scss" scoped>
.grey-text {
  color: #51534a;
}
</style>
