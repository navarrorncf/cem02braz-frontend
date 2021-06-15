<template>
  <div class="header-content">
    <div class="text">
      <p>Qualidade de <span class="highlight">ensino</span></p>
      <p>No <span class="highlight">coração</span> de Brazlândia</p>
    </div>
    <div class="button">
      <a href="#first-section">
        <button>Conheça <span class="arrow">➔</span></button>
      </a>
    </div>
    <div class="tree">
      <img src="../../assets/images/cem02-tree.png" alt="" />
    </div>
  </div>
</template>

<script>
export default {
  name: "HeaderContent",
};
</script>

<style scoped>
.header-content {
  height: calc(100vh - 60px);
  width: 50%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  color: #5d5246;
  text-align: center;
  font-variation-settings: "wght" 475;
}

.header-content .text {
  font-size: 3rem;
  margin-bottom: 4rem;
}

.header-content .button {
  margin-bottom: 4rem;
  margin-top: -1rem;
}

.header-content p {
  line-height: 1;
  margin: 1.5rem 0;
}

.header-content p:first-child {
  animation: fade-in-left 1.2s cubic-bezier(0.23, 1, 0.32, 1) 0.3s backwards;
}

.header-content p:last-child {
  animation: fade-in-right 1.2s cubic-bezier(0.23, 1, 0.32, 1) 1.2s backwards;
}

.header-content p .highlight {
  color: #7c6e4c;
  font-size: 4.8rem;
  font-variation-settings: "wght" 250;
}

button {
  animation: fade-in 1.2s cubic-bezier(0.23, 1, 0.32, 1) 2.1s backwards;
  background: transparent;
  padding: 1rem 2rem;
  border: solid 2px #7c6e4c;
  border-radius: 5px;
  color: #7c6e4c;
  font-size: 2.5rem;
  font-variation-settings: "wght" 450;
  font-family: inherit;
  cursor: pointer;
  transition: all 0.3s;
}

button:hover {
  border: solid 2px #5d5246;
  color: #5d5246;
}

button .arrow {
  display: inline-block;
  transition: transform 0.3s;
  backface-visibility: hidden;
  -moz-backface-visibility: hidden;
  -webkit-backface-visibility: hidden;
}

button:hover .arrow {
  transform: rotate(90deg);
}

.header-content .tree {
  margin: 1rem 0;
  opacity: 0.8;
  height: 20rem;
  filter: drop-shadow(0px 5px 6px #0005);
}

.header-content .tree img {
  height: 100%;
}

@keyframes fade-in-left {
  0% {
    opacity: 0;
    transform: translateX(-80px);
  }

  100% {
    opacity: 1;
    transform: translateX(0);
  }
}

@keyframes fade-in-right {
  0% {
    opacity: 0;
    transform: translateX(80px);
  }

  100% {
    opacity: 1;
    transform: translateX(0);
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
  }

  100% {
    opacity: 1;
  }
}
</style>
