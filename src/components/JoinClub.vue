<template>
  <div class="py-10 page-container">
    <v-card
      class="pa-5"
      style="box-shadow: 0 18px 45px 0 rgb(0 0 0 / 13%); width: 80%; margin: 0 auto;"
    >
      <div class="font-weight-medium">JOIN THE CL CLUB!</div>
      <div class="d-flex">
        <input class="input-style" type="text" placeholder="email address" />
        <div class="btn">
          <v-icon style="padding-top: 10px;" color="white">mdi-chevron-right</v-icon>
        </div>
      </div>
    </v-card>
  </div>
</template>

<script>
export default {};
</script>

<style scoped lang="scss">
.page-container {
  max-width: 1000px;
  margin: 0 auto;
  border-radius: 5px;
}
.input-style {
  width: 100%;
  margin-top: 10px;
  padding: 10px 10px;
  background-color: #f4f4f7;
}
.input-style:hover {
  border-left: 4px solid #cccccf;
  outline: none;
}
.input-style:focus {
  border-left: 4px solid #7a7a7b;
  outline: none;
}
.btn {
  margin-top: 10px;
  background-color: #494b43;
  padding: 0px 12px;
  cursor: pointer;
}
</style>