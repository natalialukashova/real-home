<template>
  <div class="home">
    <Carousel />
    <MainContainer>
    </MainContainer>
  </div>
</template>

<script>
// @ is an alias to /src
import MainContainer from '../components/MainContainer'
import Carousel from '../components/Carousel'

export default {
  name: 'Home',
  components: {
    MainContainer,
    Carousel,
  }
}
</script>
