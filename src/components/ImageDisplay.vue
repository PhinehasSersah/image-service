<template>
  <div class="section">
    <div
      v-for="(image, index) in getImageUrl"
      :key="index"
      class="image-display"
    >
      <img class="shoe" :src="image" alt="top sneaker"  lazy-load="true"/>
    </div>
    <!-- <h1>Top Rated Sneaker</h1> -->
  </div>
</template>

<script>
export default {
  name: "ImageDisplay",
  computed: {
    getImageUrl() {
      return [
        "https://a.storyblok.com/f/157001/3806x4757/e7769470fd/oguz-yagiz-kara-j_czzagnjjm-unsplash.jpg/m/",
        "https://a.storyblok.com/f/157001/1920x2880/4b564b118e/usama-akram-s-gyabqtoxk-unsplash.jpg",
        "https://a.storyblok.com/f/157001/4000x6000/13f6884d97/ryan-plomp-76w_edo1u1e-unsplash.jpg",
        "https://a.storyblok.com/f/157001/7016x4960/bee31a05c8/kris-gerhard-0bkzfcamvgg-unsplash.jpg",
        "https://a.storyblok.com/f/157001/640x960/47d1711332/erik-mclean-e_qqxymdyfm-unsplash.jpg",
        "https://a.storyblok.com/f/157001/6016x4016/97766bdb18/chuttersnap-clawroztlag-unsplash.jpg",
        "https://a.storyblok.com/f/157001/4160x5200/c8d80e3406/ox-street-na5zudycqas-unsplash.jpg",
        "https://a.storyblok.com/f/157001/3456x5184/535aa76dc9/pauline-figuet-4qdkcsxdo1s-unsplash.jpg",
      ];
      //   let imageUrl =
    },
  },
};
</script>

<style scoped>
.section {
  display: grid;
  grid-template-columns: 2fr 1fr;
  gap: 6%;
}
.image-display {
  display: block;
  margin: 0 auto;
  width: 40vw;
  height: 40vw;
}
.shoe {
  width: 100%;
  height: 100%;
  object-fit: cover;
 
}
h1 {
  font-size: 2em;
  margin-top: 12px;
}
</style>
