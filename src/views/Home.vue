<template>
  <div class="home">
    <!-- Title and Impression for AlgoJS Project -->
    <v-img height="500" src="https://wallpapercave.com/wp/wp3621084.jpg">
      <v-layout
        column
        align-center
        justify-center
        class="lightbox white--text pa-2 fill-height text-center"
      >
        <div class="display-1">Join Hobby Community for Algorithms</div>
        <div class="title">
          In
          <span class="display-2 yellow--text">JS</span>
        </div>

        <v-btn x-large color="teal white--text ma-4">Join Now</v-btn>
      </v-layout>
    </v-img>

    <!-- Introduction to AlgoJs Project -->
    <v-container>
      <v-row>
        <h2 class="title pt-10">Why?</h2>
        <p
          class="content pt-4"
        >စိတ်ပါဝင်စားပီး တကယ်လေ့လာနေတဲ့သူတွေ ဝင်ရောက်ကြည့်ရှူနိုင်စေရန်ရည်ရွယ်ထားပါတယ်။ လောလောဆယ်တော့ လေ့လာဆဲမို့ အများကြီးမတင်နိုင်ပါဘူး။ အမှားများနိုင်ပါတယ်။ သိတဲ့သူများဝေဖန်ထောက်ပြပေးနိုင်ပါတယ်။ နောက်ပိုင်း discussion feature လေးထည့်နိုင်အောင်ကြိုးစားပါဦးမယ်။ စိတ်ပါဝင်စားသူများ အကြံဉာဏ်များပေးနိုင်ပါတယ်။</p>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  name: "Home"
};
</script>

<style scoped>
.lightbox {
  box-shadow: 0 0 20px inset rgba(0, 0, 0, 0.2);
  background-image: linear-gradient(
    to top,
    rgba(0, 0, 0, 0.473) 100%,
    transparent 72px
  );
}
</style>
