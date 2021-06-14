<template>
  <nav class="main-navigation">
    <div class="title">CEM02BRAZ</div>
    <div class="nav-menu">
      <ul>
        <li>
          <router-link to="/">Início</router-link>
        </li>
        <li>
          <router-link to="/">Aluno</router-link>
        </li>
        <li>
          <router-link to="/">Eventos</router-link>
        </li>
        <li>
          <router-link to="/">Sobre Nós</router-link>
        </li>
        <li>
          <router-link to="/">Atendimento</router-link>
        </li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  name: "NavigationMenu",
  data() {
    return {
      lastScroll: null,
      navElement: null,
    };
  },
  methods: {
    handleScroll() {
      const pageYoffset = window.top.scrollY;

      if (this.lastScroll < pageYoffset) {
        this.hide();
      } else {
        this.show();
      }

      this.lastScroll = pageYoffset;
    },
    hide() {
      this.navElement.classList.add("hidden");
    },
    show() {
      this.navElement.classList.remove("hidden");
    },
  },
  created() {
    window.addEventListener("scroll", this.handleScroll);
  },
  mounted() {
    this.navElement = document.querySelector(".main-navigation");
  },
};
</script>

<style>
nav.main-navigation {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  display: flex;
  height: 6rem;
  background: #e4e2deaa;
  justify-content: space-between;
  align-items: center;
  padding: 0 2rem;
  color: #5d5246;
  font-variation-settings: "wght" 450;
  transition: transform 0.6s;
  z-index: 10;
}

nav.main-navigation.hidden {
  transform: translateY(-100%);
}

nav.main-navigation .title {
  font-size: 2.8rem;
  letter-spacing: -0.5px;
}

nav.main-navigation .nav-menu {
  font-size: 2.1rem;
}

nav.main-navigation .nav-menu ul {
  list-style: none;
  display: flex;
  height: 100%;
}

nav.main-navigation .nav-menu ul li {
  margin: 0 1.5rem;
  display: flex;
  flex-direction: column;
}

nav.main-navigation .nav-menu ul li::after {
  content: "";
  position: relative;
  left: 0;
  bottom: 0.4rem;
  width: 100%;
  height: 2px;
  transform: scaleX(0);
  background: #5d5246cc;
  transition: all 0.2s;
}

nav.main-navigation .nav-menu ul li:hover::after {
  transform: scaleX(1);
}

nav.main-navigation .nav-menu ul li a {
  display: inline-block;
  padding: 0.5rem 1rem;
  transition: all 0.2s;
}

nav.main-navigation .nav-menu a:link,
nav.main-navigation .nav-menu a:visited {
  text-decoration: none;
  color: inherit;
}
</style>
