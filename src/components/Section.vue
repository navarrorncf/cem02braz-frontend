<template>
  <section class="section">
    <div class="section--content">
      <h2 class="title">
        {{ title }}
        <i v-if="fontAwesomeIconClasses" :class="fontAwesomeIconClasses"></i>
      </h2>
      <slot></slot>
    </div>
  </section>
</template>

<script>
export default {
  name: "Section",
  props: {
    title: String,
    fontAwesomeIconClasses: {
      type: String,
      default: "",
    },
  },
};
</script>

<style scoped>
.section {
  background: #e4e2de;
  color: #5d5246;
}

.section:nth-of-type(odd) {
  background: linear-gradient(to top, #e4e2de66, #e4e2de66),
    url("../assets/images/papyrus.png");
  background-attachment: fixed;
}

.section--content {
  max-width: 70rem;
  margin: 0 auto;
  padding: 6rem 0;
}

.title {
  font-size: 4.2rem;
  font-variation-settings: "wght" 375;
  margin-bottom: 4.2rem;
  font-variant: small-caps;
  letter-spacing: -1px;
  text-shadow: 0 2px 2px #5d5246;
}

.text {
  max-width: 30em;
}

.title i {
  color: #7c6e4c;
  text-shadow: 0 2px 2px #5d5246;
  margin-left: 1rem;
}

.title i.light-red {
  color: #e23232;
}
</style>
