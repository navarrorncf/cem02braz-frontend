<template>
  <Section
    id="local"
    fontAwesomeIconClasses="fas fa-map-marker-alt light-red"
    title="Venha Nos Visitar"
  >
    <div>
      <p class="text">
        O CEM02BRAZ fica Quadra 36 da Vila São José – Brazlândia, próximo ao
        Restaurante Comunitário e ao Centro Olímpico. Venha nos conhecer!
      </p>
    </div>
    <div class="google-map">
      <iframe
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2284.217932984744!2d-48.194515877933405!3d-15.667266867441567!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x935bb12b07ffffff%3A0x335a84fb5999bec3!2sCEM%2002%20de%20Brazl%C3%A2ndia!5e0!3m2!1spt-BR!2sbr!4v1623762677711!5m2!1spt-BR!2sbr"
        allowfullscreen=""
        loading="lazy"
      ></iframe>
    </div>
  </Section>
</template>

<script>
import Section from "./Section.vue";

export default {
  name: "Location",
  components: {
    Section,
  },
};
</script>

<style scoped>
.google-map {
  background: #5d5246aa;
  font-size: 1.7rem;
  width: 30em;
  height: 26em;
  padding: 0.5rem;
}

.google-map iframe {
  width: 100%;
  height: 100%;
  border: none;
}
</style>
