<template>
  <div class="home">
    <Header/>
    <Banner>
      <Title title="Best leasing deals in one place" subtitle="Our customers save on avarage 40€"/>
      <div class="banner__buttons-container">
        <Button title="here a CTA"/>
        <Button title="here a is another CTA" :modifierClasses="['ghost']"/>
      </div>
    </Banner>
    <SectionTitle title="Only on Vehiculum"/>
    <Carousel/>
    <SectionTitle title="Find leasing for your brand"/>
    <BrandLogos/>
    <PromoSection/>
    <Banner>
      <DetailsTable modifierClass="boxed"/>
      <div class="banner__buttons-container">
        <Button title="Last 2 cars available" :modifierClasses="['red', 'fullwidth']"/>
      </div>
    </Banner>
  </div>
</template>

<script>
// @ is an alias to /src
import RatingBox from "@/components/atoms/RatingBox.vue";

import Banner from "@/components/molecules/Banner.vue";
import Carousel from "@/components/organisms/Carousel.vue";
import Title from "@/components/atoms/Title.vue";
import Button from "@/components/atoms/Button.vue";
import Header from "@/components/organisms/Header.vue";
import SectionTitle from "@/components/atoms/SectionTitle.vue";
import DetailsTable from "@/components/atoms/DetailsTable.vue";
import PromoSection from "@/components/molecules/PromoSection.vue";
import BrandLogos from "@/components/molecules/BrandLogos.vue";

export default {
  name: "home",
  components: {
    Header,
    Banner,
    SectionTitle,
    RatingBox,
    Carousel,
    Title,
    Button,
    DetailsTable,
    PromoSection,
    BrandLogos
  }
};
</script>
