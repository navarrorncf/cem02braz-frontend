<template>
  <Section
    id="atendimento"
    title="Atendimento"
    fontAwesomeIconClasses="far fa-comment-dots"
  >
    <div class="contact">
      <p class="text">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ullam nulla
        distinctio aperiam vitae eum, voluptatum numquam laborum fugiat tempore
        provident voluptas reiciendis enim vel necessitatibus.
      </p>
      <h3>Secretaria Escolar</h3>
      <p class="text description">
        Para matrículas, transferências, declarações e documentos:
      </p>
      <ul class="contact-info">
        <li>
          <i class="fab fa-whatsapp-square"></i>
          <span class="contact">Whatsapp: </span>
          <a href="https://api.whatsapp.com/send?phone=+556139013692"
            >(61) 3901-3692</a
          >
        </li>
        <li>
          <i class="fa fa-envelope-open-text"></i>
          <span class="contact">Email: </span>
          <a
            href="mailto:cem02.brazlandia@edu.se.df.gov.br?subject=Preciso de ajuda"
            >cem02.brazlandia@edu.se.df.gov.br</a
          >
        </li>
        <li>
          <i class="fas fa-head-side-mask"></i>
          <span class="contact">Atendimento Presencial:</span> às segundas,
          terças, quintas e sextas, das 14h às 17h.
          <strong>Não há atendimento presencial às quartas-feiras.</strong>
        </li>
      </ul>
      <hr />
      <h3>Plataforma - Google Classroom</h3>
      <p class="text description">
        Para obter email de acesso à plataforma, cadastros nas turmas, reiniciar
        senhas ou tirar dúvidas:
      </p>
      <ul class="contact-info">
        <li>
          <i class="fa fa-envelope-open-text"></i>
          <span class="contact">Email: </span>
          <a
            href="mailto:plataformacem02braz@gmail.com?subject=Preciso de ajuda"
            >plataformacem02braz@gmail.com</a
          >
        </li>
      </ul>
      <hr />
      <h3>Direção</h3>
      <p class="text description">
        Para resolução de conflitos e assuntos gerais:
      </p>
      <ul class="contact-info">
        <li>
          <i class="fab fa-whatsapp-square"></i>
          <span class="contact">Whatsapp: </span>
          <a href="https://api.whatsapp.com/send?phone=+556139013692"
            >(61) 3901-3692</a
          >
        </li>
        <li>
          <i class="fa fa-envelope-open-text"></i>
          <span class="contact">Email: </span>
          <a href="mailto:cem02braz@gmail.com?subject=Preciso de ajuda"
            >cem02braz@gmail.com</a
          >
        </li>
        <li>
          <i class="fas fa-head-side-mask"></i>
          <span class="contact">Atendimento Presencial:</span> às segundas,
          terças, quintas e sextas, das 9h às 12h ou 14h às 17h.
          <strong>Não há atendimento presencial às quartas-feiras.</strong>
        </li>
      </ul>
    </div>
  </Section>
</template>

<script>
import Section from "./Section.vue";

export default {
  name: "Contact",
  components: {
    Section,
  },
};
</script>

<style scoped>
hr {
  border: none;
  border-top: solid 1px #5d524666;
}

h3 {
  font-size: 3rem;
  font-variation-settings: "wght" 500;
  text-shadow: 0 1px 2px #5d5246aa;
  margin: 6rem 0;
}

p.text.description {
  margin: -4.5rem 0 5rem 0;
}

ul.contact-info {
  list-style: none;
  margin: -1rem 0 6rem 0;
}

ul.contact-info li {
  margin: 1.5rem 0;
  font-variation-settings: "wght" 450;
  font-size: 1.6rem;
}

ul.contact-info li i {
  font-size: 2.2rem;
  margin-right: 1rem;
  /* transform: translateY(1px); */
}

ul.contact-info li i.fab {
  font-size: 2.5rem;
  transform: translateY(3px);
}

ul.contact-info li .contact {
  font-variation-settings: "wght" 650;
  font-size: 1.8rem;
}

ul.contact-info li strong {
  font-variation-settings: "wght" 650;
}

ul.contact-info li a:link,
ul.contact-info li a:visited {
  color: inherit;
  font-variation-settings: "wght" 550;
}

.fa-envelope-open-text {
  color: #c71610;
}

.fa-whatsapp-square {
  color: #25d366;
}

.fa-head-side-mask {
  color: #126db8;
}
</style>
