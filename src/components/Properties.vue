<template>
  <div class="properties">
    <div class="container">
      <div class="row">
        <div class="col">
          <h2 class="properties__h2">Featured <span>Properties</span></h2>
        </div>
        <div class="col">
          <p class="properties__subtitle">
            Quisque diam lorem interdum vitaapibus vitae pede. Donec eget tellus
            non erat lacinia fertum. Donec in velit vel ipsum auctovinar.
          </p>
        </div>
      </div>
      <div class="row">
        <div
          class="col-md-4 col-sm-12"
          v-for="property in propertiesData"
          :key="property.id"
        >
          <div class="properties__col">
            <img
              class="properties__img"
              :src="require(`../assets/img/${property.image}.png`)"
              :alt="property.desc.title"
            />
            <h4 class="properties__h4">{{ property.title }}</h4>
            <p class="properties__sub">{{ property.subtitle }}</p>
            <p class="properties__price">{{ property.price }}</p>
            <ul class="properties__desc">
              <li class="properties__item">{{ property.desc.area }}</li>
              <li class="properties__item">{{ property.desc.rooms }}</li>
              <li class="properties__item">{{ property.desc.bath }}</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col">
        <button type="button" class="btn btn-primary properties__more">All properties</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    propertiesData: {
      type: Array,
      default: () => [],
    },
  },
};
</script>