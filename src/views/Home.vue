<template>
    <div>
        <OwlCarousel />
        <Services/>
        <Category/>
        <FeaturedProduct/>
    </div>
</template>

<script>

import OwlCarousel from "@/components/home-content/OwlCarousel";
import Services from "@/components/home-content/Services";
import Category from "@/components/home-content/Category";
import FeaturedProduct from "@/components/home-content/FeaturedProduct";
export default {
  name: 'Home',
  components: {
      FeaturedProduct,
      Category,
      Services,
      OwlCarousel
  }
}
</script>
