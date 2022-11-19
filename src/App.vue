<template>
  <div>
    <HeaderLayout fonts="GmarketSans" />
    <SliderSection fonts="GmarketSans" />
    <TextSection attr="section GmarketSans" layout="container" />
    <CardSection attr="section GmarketSans" layout="container" />
    <ImageSection attr="section GmarketSans" layout="container" />
    <BannerSection fonts="GmarketSans" />
    <ImgTextSection attr="section GmarketSans" layout="container" />
    <FooterLayout attr="section nexon gray" layout="container" />
  </div>
</template>

<script>
import HeaderLayout from "./components/layout/HeaderLayout.vue";
import FooterLayout from "./components/layout/FooterLayout.vue";
import ImageSection from "./components/section/ImageSection.vue";
import ImgTextSection from "./components/section/ImgTextSection.vue";
import SliderSection from "./components/section/SliderSection.vue";
import TextSection from "./components/section/TextSection.vue";
import BannerSection from "./components/section/BannerSection.vue";
import CardSection from "./components/section/CardSection.vue";

export default {
  name: "App",
  components: {
    HeaderLayout,
    SliderSection,
    TextSection,
    CardSection,
    ImageSection,
    BannerSection,
    ImgTextSection,
    FooterLayout,
  },
};
</script>
