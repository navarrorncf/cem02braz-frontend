<template>
  <nav class="main-navigation">
    <div class="title">CEM02BRAZ</div>
    <div class="nav-menu">
      <ul>
        <li>
          <a href="/#top">Início</a>
        </li>
        <li class="submenu">
          <span>Informações <i class="fa fa-angle-down"></i></span>
          <div class="submenu">
            <ul>
              <li>
                <router-link to="/aluno">Área do Aluno</router-link>
              </li>
              <li>
                <router-link to="/eventos">Eventos</router-link>
              </li>
            </ul>
          </div>
        </li>
        <li class="submenu">
          <span>Fale Conosco <i class="fa fa-angle-down"></i></span>
          <div class="submenu">
            <ul>
              <li>
                <a href="/#atendimento">Atendimento</a>
              </li>
              <li>
                <a href="/#local">Localização</a>
              </li>
            </ul>
          </div>
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
  visibility: hidden;
  opacity: 0;
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

nav.main-navigation .nav-menu ul ul {
  flex-direction: column;
  padding-top: 1.2rem;
  text-align: center;
  height: unset;
  padding-bottom: 1rem;
  background: #e4e2debb;
}

nav.main-navigation .nav-menu ul div.submenu {
  position: absolute;
  top: 100%;
  right: 0%;
  padding-top: 1.2rem;
  visibility: hidden;
}

nav.main-navigation .nav-menu ul li.submenu {
  cursor: pointer;
}

li.submenu i {
  transform: translateY(3px);
}

nav.main-navigation .nav-menu ul ul li a {
  padding: 1rem 1.5rem;
  transition: all 0s;
}

nav.main-navigation .nav-menu ul ul li {
  padding: 0 2rem;
  white-space: nowrap;
}

nav.main-navigation .nav-menu ul ul li {
  margin: 0 1rem;
}

nav.main-navigation .nav-menu ul li.submenu:hover * {
  visibility: visible;
}

nav.main-navigation .nav-menu ul li {
  margin: 0 1.5rem;
  display: flex;
  flex-direction: column;
  justify-content: center;
  cursor: pointer;
  position: relative;
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

nav.main-navigation .nav-menu ul li a,
nav.main-navigation .nav-menu ul li span {
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
