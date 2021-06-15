<template>
  <div class="footer-container">
    <footer>
      <div class="social">
        <h3>
          CEM02BRAZ &ndash; Links <i class="fas fa-external-link-alt"></i>
        </h3>
        <p class="text">Siga-nos nas nossas redes sociais!</p>
        <ul>
          <li>
            <a
              href="http://facebook.com/cem02braz"
              class="facebook"
              target="_blank"
              rel="noopener noreferrer"
            >
              <i class="fab fa-facebook-square"></i>
              Facebook
            </a>
          </li>
          <li>
            <a
              href="http://instagram.com/cem02braz"
              class="instagram"
              target="_blank"
              rel="noopener noreferrer"
            >
              <i class="fab fa-instagram-square"></i>
              Instagram
            </a>
          </li>
          <li>
            <a
              href="http://twitter.com/cem02braz"
              class="twitter"
              target="_blank"
              rel="noopener noreferrer"
            >
              <i class="fab fa-twitter-square"></i>
              Twitter
            </a>
          </li>
          <li>
            <a
              href="http://youtube.com/cem02braz"
              class="youtube"
              target="_blank"
              rel="noopener noreferrer"
            >
              <i class="fab fa-youtube-square"></i>
              YouTube
            </a>
          </li>
        </ul>
      </div>
      <hr />
      <div class="disclaimer">
        Feito com <span class="love"><i class="fas fa-heart"></i></span> no
        Centro de Ensino Médio 02 de Brazlândia
      </div>
      <div class="copy">Brasília ‒ {{ new Date().getFullYear() }}</div>
      <hr />
      <div class="developer">
        <p>
          Gostou desta página? Conheça o desenvolvedor
          <a
            href="http://navarrodev.com"
            target="_blank"
            rel="noopener noreferrer"
            >clicando aqui</a
          >
          e peça um website para o seu negócio!
        </p>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped>
.footer-container {
  padding: 3rem 0;
  background: #e4e2deaa;
  color: #5d5246;
  border-top: solid 1px #5d524644;
}

footer {
  max-width: 60rem;
  margin: 0 auto;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
  font-size: 1.6rem;
  font-variation-settings: "wght" 475;
}

footer > * {
  width: 100%;
}

.disclaimer .love {
  color: rgb(255, 72, 72);
}

.social p.text {
  margin: 0 auto;
}

.social h3 {
  margin-bottom: 2rem;
}

.social,
.developer {
  margin: 3rem 0;
}

.disclaimer {
  margin: 3rem 0 1rem 0;
}

.copy {
  margin-bottom: 3rem;
}

hr {
  width: 200px;
  border: none;
  border-top: solid 1px #5d524666;
}

.social h3 {
  font-size: 2.8rem;
  text-transform: uppercase;
  font-variation-settings: "wght" 500;
  text-shadow: 0 1px 1px #5d5246;
}

.social h3 i {
  color: #7c6e4c;
  margin-left: 1rem;
}

.social ul {
  list-style: none;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-top: 3rem;
  font-size: 2rem;
}

.social ul li {
  margin: 0 2rem;
}

.social ul li a {
  transition: all 0.3s;
  font-size: 1.8rem;
}

.social ul li .fab {
  font-size: 2.2rem;
  transform: translateY(1px);
  margin-right: 0.2rem;
}

.social ul li:hover a.facebook {
  color: #1877f2;
}

.social ul li:hover a.instagram {
  color: #c32aa3;
}

.social ul li:hover a.twitter {
  color: #1da1f2;
}

.social ul li:hover a.youtube {
  color: #ff0000;
}

a:link,
a:visited {
  color: inherit;
  text-decoration: none;
}

.developer p {
  text-align: left;
  color: #5d5246cc;
  font-size: 1.6rem;
}

.developer a {
  color: #7c6e4cdd;
  font-variation-settings: "wght" 600;
  text-decoration: underline;
}
</style>
