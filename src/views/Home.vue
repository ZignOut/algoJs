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
        <h2 class="title mt-10">Why?</h2>
        <p
          class="content mt-4"
        >စိတ်ပါဝင်စားပီး တကယ်လေ့လာနေတဲ့ သူတွေ ဝင်ရောက်ကြည့်ရှူနိုင် စေရန်ရည်ရွယ်ထား ပါတယ်။ လောလောဆယ်တော့ လေ့လာဆဲမို့ အများကြီး မတင်နိုင်ပါဘူး။ အမှားများနိုင် ပါတယ်။ သိတဲ့သူများ ဝေဖန်ထောက်ပြ ပေးနိုင်ပါတယ်။ နောက်ပိုင်း discussion feature လေးထည့်နိုင် အောင်ကြိုးစားပါ ဦးမယ်။ စိတ်ပါဝင်စားသူများ အကြံဉာဏ်များ ပေးနိုင်ပါတယ်။</p>

        <h2 class="title mt-10 d-block">Featuring</h2>

        <v-card :href="feature.link" v-for="feature in features" :key="feature" width="300px" color="white darken-4 teal--text" class=" d-inline-block pt-4 mt-6 mr-md-12">
          <v-card-title>{{ feature.title }}</v-card-title>
          <v-card-subtitle>Author. {{ feature.author }}</v-card-subtitle>
          <div class="pt-4">
            <v-btn class="pl-6" icon>
              <v-icon>star</v-icon>
              <span>{{ feature.like }}</span>
            </v-btn>

            <v-btn class="pl-10" icon>
              <v-icon>comment</v-icon>
              <span>{{ feature.comment }}</span>
            </v-btn>
          </div>
        </v-card>
    </v-container>
  </div>
</template>

<script>
export default {
  name: "Home",

  data() {
    return {
      features: [
        {
          title: 'Merge Sort',
          author: 'kaunghtut',
          like: 5,
          comment: 6,
          link: '/mergesort'
        },
        {
          title: 'Selection Sort',
          author: 'kaunghtut',
          like: 2,
          comment: 9,
          link: '/selectionsort'
        },
        {
          title: 'Selection Sort',
          author: 'kaunghtut',
          like: 2,
          comment: 9,
          link: '/selectionsort'
        },
        {
          title: 'Selection Sort',
          author: 'kaunghtut',
          like: 2,
          comment: 9,
          link: '/selectionsort'
        },
        {
          title: 'Selection Sort',
          author: 'kaunghtut',
          like: 2,
          comment: 9,
          link: '/selectionsort'
        },
        {
          title: 'Selection Sort',
          author: 'kaunghtut',
          like: 2,
          comment: 9,
          link: '/selectionsort'
        },
        {
          title: 'Selection Sort',
          author: 'kaunghtut',
          like: 2,
          comment: 9,
          link: '/selectionsort'
        },
      ]
    }
  }
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
