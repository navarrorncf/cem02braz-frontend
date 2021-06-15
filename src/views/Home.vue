<template>
  <Header />
  <Section id="first-section" title="Um Pouco Sobre Nós">
    <p class="text">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. In suscipit,
      incidunt quisquam autem, harum sequi, eius perspiciatis quis enim
      voluptatem placeat voluptates quos repellendus molestias explicabo?
      Dolore, voluptates quas reiciendis expedita quae impedit accusantium,
      repudiandae officiis cupiditate itaque natus porro.
    </p>
    <p class="text">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Hic omnis non in
      facilis eligendi laboriosam voluptatibus odio porro adipisci quam, minima
      qui dolorem maiores repudiandae molestiae ea modi asperiores ut et
      possimus minus officiis. Ullam, reiciendis doloribus in quia tenetur sunt
      ipsam consectetur, similique aut id magnam? Omnis, reprehenderit dolor.
    </p>
  </Section>
  <Section title="Nossos Valores">
    <p class="text">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. In suscipit,
      incidunt quisquam autem, harum sequi, eius perspiciatis quis enim
      voluptatem placeat voluptates quos repellendus molestias explicabo?
      Dolore, voluptates quas reiciendis expedita quae impedit accusantium,
      repudiandae officiis cupiditate itaque natus porro.
    </p>
    <p class="text">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Hic omnis non in
      facilis eligendi laboriosam voluptatibus odio porro adipisci quam, minima
      qui dolorem maiores repudiandae molestiae ea modi asperiores ut et
      possimus minus officiis. Ullam, reiciendis doloribus in quia tenetur sunt
      ipsam consectetur, similique aut id magnam? Omnis, reprehenderit dolor.
    </p>
  </Section>
  <Section title="Venha Conhecer">
    <p class="text">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. In suscipit,
      incidunt quisquam autem, harum sequi, eius perspiciatis quis enim
      voluptatem placeat voluptates quos repellendus molestias explicabo?
      Dolore, voluptates quas reiciendis expedita quae impedit accusantium,
      repudiandae officiis cupiditate itaque natus porro.
    </p>
    <p class="text">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Hic omnis non in
      facilis eligendi laboriosam voluptatibus odio porro adipisci quam, minima
      qui dolorem maiores repudiandae molestiae ea modi asperiores ut et
      possimus minus officiis. Ullam, reiciendis doloribus in quia tenetur sunt
      ipsam consectetur, similique aut id magnam? Omnis, reprehenderit dolor.
    </p>
  </Section>
  <Footer />
</template>

<script>
// @ is an alias to /src
import Header from "@/components/header/Header";
import Section from "@/components/Section";
import Footer from "@/components/Footer";

export default {
  name: "Home",
  components: {
    Header,
    Section,
    Footer,
  },
};
</script>
