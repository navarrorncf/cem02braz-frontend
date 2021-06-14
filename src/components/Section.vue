<template>
  <div class="section">
    <div class="section--content">
      <h2 class="title">{{ title }}</h2>
      <slot></slot>
    </div>
  </div>
</template>

<script>
export default {
  name: "Section",
  props: {
    title: String,
  },
};
</script>

<style scoped>
.section {
  background: #e4e2de;
  color: #5d5246;
}

.section:nth-of-type(even) {
  background: #f5f3ef;
}

.section--content {
  max-width: 60rem;
  margin: 0 auto;
  padding: 6rem 0;
}

.title {
  font-size: 4.2rem;
  font-variation-settings: "wght" 550;
  margin-bottom: 4.2rem;
  font-variant: small-caps;
  letter-spacing: -1px;
}

.text {
  max-width: 30em;
}
</style>
