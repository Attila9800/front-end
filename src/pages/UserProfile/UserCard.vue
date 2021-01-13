<template>
  <md-card class="md-card-profile">
    <div class="md-card-avatar">
      <img class="img" :src="cardUserImage" />
    </div>

    <md-card-content>
      <h6 class="category text-gray">Software Engineer</h6>
      <h4 class="card-title">KOSSYN YEDIL</h4>
      <p class="card-description">
        Studen of TianJin Univercity software school
      </p>
      <md-button class="md-round md-success">Follow</md-button>
    </md-card-content>
  </md-card>
</template>
<script>
export default {
  name: "user-card",
  props: {
    cardUserImage: {
      type: String,
      default: require("@/assets/img/faces/attila2.jpg")
    }
  },
  data() {
    return {};
  }
};
</script>
<style></style>
