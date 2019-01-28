<template>
  <div class="home">
    <my-header></my-header>
    <my-features></my-features>
    <my-aboutus></my-aboutus>
    <my-about-us-discriptions></my-about-us-discriptions>
    <my-services></my-services>
    <my-how-we-work></my-how-we-work>
    <my-work-progress></my-work-progress>
  </div>
</template>

<script>
// @ is an alias to /src
import Header from '../components/Header'
import Features from '../components/Features'
import AboutUs from "../components/AboutUs";
import AboutUsDiscriptions from "../components/AboutUsDiscriptions";
import OurServices from "../components/OurServices";
import HowWeWork from "../components/HowWeWork";
import WorkProgress from "../components/WorkProgress";

export default {
  name: 'home',
  components: {
    AboutUs,
    'my-header' : Header,
    'my-features':Features,
    'my-aboutus':AboutUs,
    'my-about-us-discriptions':AboutUsDiscriptions,
    'my-services':OurServices,
    'my-how-we-work':HowWeWork,
    'my-work-progress':WorkProgress,
  }
}

</script>

<style lang="scss">

</style>

