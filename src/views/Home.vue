<template>
  <div class="home">
    <Carousel />
    <div class="container home__offering">
      <div class="row">
        <div class="col-md-4  home_border">
          <h3 class="home__offering-title">We are Offering the Best Estate Deals</h3>
        </div>
        <div class="col-md-8">
          <p class="home__paragraph">
            Quisque diam lorem interdum vitaapibus ac scelerisque vitae pede.
            Donec eget tellus non erat lacinia fertum. Donec in velit vel ipsum
            auctovinar. Proin umcorper urna et felisstibulum iaculis lacinia
            est. Proin dictum elem entum velit fusce euismod. Aenean commodo
            ligula eget dolor. Aenean massa. Lorem ipsum dolor sit amet, consec
            tetuer adipis elit, aliquam eget nibh etlibura. Lorem ipsum dolor
            sitamet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor
            invidunt ut labore et.
          </p>
        </div>
      </div>
    </div>
    <Feauters :data="feautereData" />
    <Properties :propertiesData="propertiesData" />
  </div>
</template>

<script>
// @ is an alias to /src
import Carousel from "../components/Carousel";
import Feauters from "../components/Feauters"
import Properties from "../components/Properties"
import { feautereData } from "../data/data.feauters"
import { propertiesData } from "../data/data.properties"

export default {
  name: "Home",
  components: {
    Carousel,
    Feauters,
    Properties,
  },
  data() {
    return {
      feautereData: feautereData,
      propertiesData: propertiesData,
    }
  },
};
</script>
