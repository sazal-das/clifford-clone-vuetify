<template>
  <v-card
    v-if="screenWidth >= 1000"
    :style="dark ? 'box-shadow: 0 18px 45px 0 rgb(0 0 0 / 13%); background-color: #333333;' : 'box-shadow: 0 18px 45px 0 rgb(0 0 0 / 13%);'"
    class="page-container"
  >
    <div class="text-center">
      <v-avatar
        style="box-shadow: 0 18px 45px 0 rgb(0 0 0 / 13%);"
        size="120px"
        class="profile-image"
      >
        <img :src="`images/profile/${profile.imageSrc}`" />
      </v-avatar>
      <div
        class="my-4 font-weight-bold text-h5 d-flex text-center"
        :class="dark ? 'white--text' : ''"
        style="width: max-content; margin: 0 auto;"
      >
        <div>{{ profile.name }}</div>
        <div style="width: 20px" class="mt-2 ml-1" v-if="solo">
          <v-img color="black" src="/images/social/verified.svg"></v-img>
        </div>
      </div>
      <div class="my-4 grey--text">
        <v-icon color="#B1B1B1">mdi-map-marker-outline</v-icon>
        {{ profile.address }}
      </div>
      <div class="my-4" :class="dark ? 'white--text' : ''">{{ profile.info }}</div>
      <div>
        <v-btn tile outlined color="#B1B1B1">
          <v-icon :color="dark ? 'white' : 'black'" left>mdi-email</v-icon>
          <span class="text-capitalize black--text" :class="dark ? 'white--text' : ''">Email</span>
        </v-btn>
      </div>
      <div class="my-4" v-if="solo">
        <v-btn fab class="mx-2" outlined small color="#B1B1B1">
          <v-icon color="white">mdi-instagram</v-icon>
        </v-btn>
        <v-btn fab class="mx-2" outlined small color="#B1B1B1">
          <v-icon color="white">mdi-twitter</v-icon>
        </v-btn>
        <v-btn fab class="mx-2" outlined small color="#B1B1B1">
          <v-img width="8px" style="fill: white" color="black" src="/images/social/tiktok-min.svg"></v-img>
        </v-btn>
        <v-btn fab class="mx-2" outlined small color="#B1B1B1">
          <v-icon color="white">mdi-youtube</v-icon>
        </v-btn>
        <v-btn fab class="mx-2" outlined small color="#B1B1B1">
          <v-icon color="white">mdi-twitch</v-icon>
        </v-btn>
      </div>
      <div class="my-4" v-else>
        <v-btn fab class="mx-2" outlined small color="#B1B1B1">
          <v-img width="8px" color="black" src="/images/social/website.svg"></v-img>
        </v-btn>
        <v-btn fab class="mx-2" outlined small color="#B1B1B1">
          <v-img width="8px" color="black" src="/images/social/linkedin.svg"></v-img>
        </v-btn>
        <v-btn fab class="mx-2" outlined small color="#B1B1B1">
          <v-img width="8px" color="black" src="/images/social/facebook.svg"></v-img>
        </v-btn>
        <v-btn fab class="mx-2" outlined small color="#B1B1B1">
          <v-img width="8px" color="black" src="/images/social/tiktok.svg"></v-img>
        </v-btn>
        <v-btn fab class="mx-2" outlined small color="#B1B1B1">
          <v-img width="8px" color="black" src="/images/social/instagram.svg"></v-img>
        </v-btn>
      </div>
    </div>
  </v-card>
  <v-card
    v-else
    flat
    :style="dark ? 'background-color: #242424;' : 'background-color: #F4F4F7'"
    class="page-container"
  >
    <div class="text-center">
      <v-avatar
        style="box-shadow: 0 18px 45px 0 rgb(0 0 0 / 13%);"
        size="120px"
        class="profile-image"
      >
        <img :src="`images/profile/${profile.imageSrc}`" />
      </v-avatar>
      <div
        class="my-4 font-weight-bold text-h5 d-flex text-center"
        :class="dark ? 'white--text' : ''"
        style="width: max-content; margin: 0 auto;"
      >
        <div>{{ profile.name }}</div>
        <div style="width: 20px" class="mt-2 ml-1" v-if="solo">
          <v-img color="black" src="/images/social/verified.svg"></v-img>
        </div>
      </div>
      <div class="my-4 grey--text">
        <v-icon color="#B1B1B1">mdi-map-marker-outline</v-icon>
        {{ profile.address }}
      </div>
      <div class="my-4" :class="dark ? 'white--text' : ''">{{ profile.info }}</div>
      <div>
        <v-btn tile outlined color="#B1B1B1">
          <v-icon :color="dark ? 'white' : 'black'" left>mdi-email</v-icon>
          <span class="text-capitalize black--text" :class="dark ? 'white--text' : ''">Email</span>
        </v-btn>
      </div>
      <div class="my-4" v-if="solo">
        <v-btn fab class="mx-2" outlined small color="#B1B1B1">
          <v-icon color="white">mdi-instagram</v-icon>
        </v-btn>
        <v-btn fab class="mx-2" outlined small color="#B1B1B1">
          <v-icon color="white">mdi-twitter</v-icon>
        </v-btn>
        <v-btn fab class="mx-2" outlined small color="#B1B1B1">
          <v-img width="2" style="fill: white" color="black" src="/images/social/tiktok-min.svg"></v-img>
        </v-btn>
        <v-btn fab class="mx-2" outlined small color="#B1B1B1">
          <v-icon color="white">mdi-youtube</v-icon>
        </v-btn>
        <v-btn fab class="mx-2" outlined small color="#B1B1B1">
          <v-icon color="white">mdi-discord</v-icon>
        </v-btn>
        <v-btn fab class="mx-2" outlined small color="#B1B1B1">
          <v-icon color="white">mdi-twitch</v-icon>
        </v-btn>
      </div>
      <div class="my-4" v-else>
        <v-btn fab class="mx-2" outlined small color="#B1B1B1">
          <v-img width="8px" color="black" src="/images/social/website.svg"></v-img>
        </v-btn>
        <v-btn fab class="mx-2" outlined small color="#B1B1B1">
          <v-img width="8px" color="black" src="/images/social/linkedin.svg"></v-img>
        </v-btn>
        <v-btn fab class="mx-2" outlined small color="#B1B1B1">
          <v-img width="8px" color="black" src="/images/social/facebook.svg"></v-img>
        </v-btn>
        <v-btn fab class="mx-2" outlined small color="#B1B1B1">
          <v-img width="8px" color="black" src="/images/social/tiktok.svg"></v-img>
        </v-btn>
        <v-btn fab class="mx-2" outlined small color="#B1B1B1">
          <v-img width="8px" color="black" src="/images/social/instagram.svg"></v-img>
        </v-btn>
      </div>
    </div>
  </v-card>
</template>

<script>
export default {
  name: "ProfileSection",
  props: {
    profile: {
      type: Object,
      required: true,
    },
    dark: {
      type: Boolean,
      required: false,
      default: false,
    },
    solo: {
      type: Boolean,
      required: false,
      default: false,
    },
  },
  computed: {
    screenWidth() {
      return this.$vuetify.breakpoint.width;
    },
  },
};
</script>

<style scoped lang="scss">
.page-container {
  max-width: 1000px;
  margin: 0 auto;
  border-radius: 5px;
  margin-top: -180px;
  padding-bottom: 15px;
}
.profile-image {
  margin-top: -40px;
}
</style>