<template>
    <div>
        <OwlCarousel />
        <Services/>
        <Category/>
        <FeaturedProduct/>
        <DayOffer/>
        <Testimony/>
        <Partner/>
        <Newsletter/>
    </div>
</template>

<script>

import OwlCarousel from "@/components/home-content/OwlCarousel";
import Services from "@/components/home-content/Services";
import Category from "@/components/home-content/Category";
import FeaturedProduct from "@/components/home-content/FeaturedProduct";
import DayOffer from "@/components/home-content/DayOffer";
import Testimony from "@/components/home-content/Testimony";
import Partner from "@/components/home-content/Partner";
import Newsletter from "@/components/home-content/Newsletter";
export default {
  name: 'Home',
  components: {
      Newsletter,
      Partner,
      Testimony,
      DayOffer,
      FeaturedProduct,
      Category,
      Services,
      OwlCarousel
  }
}
</script>
