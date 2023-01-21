<template>
  <div>
    <v-card
      :style="dark ? 'box-shadow: 0 18px 45px 0 rgb(0 0 0 / 13%); background-color: #333333' : 'box-shadow: 0 18px 45px 0 rgb(0 0 0 / 13%);'"
      class="d-flex justify-space-between py-2"
    >
      <div class="d-flex">
        <v-img
          width="60"
          style="border-radius: 3px; margin-left: -15px;"
          :src="`images/item/${item.image}`"
        ></v-img>
        <div class="pt-2 pl-5" style="overflow: hidden; text-overflow: ellipsis; ">
          <div class="font-weight-medium" :class="dark ? 'white--text' : ''">{{ item.name }}</div>
          <div class="text-caption grey--text">{{ item.description }}</div>
        </div>
      </div>
      <div class="text-right pt-3">
        <v-btn icon color="grey">
          <v-icon>mdi-arrow-right-thin</v-icon>
        </v-btn>
      </div>
    </v-card>
  </div>
</template>

<script>
export default {
  name: "ItemCard",
  props: {
    item: {
      type: Object,
      required: true,
    },
    dark: {
      type: Boolean,
      required: false,
      default: false,
    },
  },
};
</script>

<style>
.bg {
  background-color: #333333;
}
</style>