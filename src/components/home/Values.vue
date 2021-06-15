<template>
  <div class="values">
    <div class="cards">
      <div class="card student">
        <div class="content">
          <div class="title">Foco no estudante</div>
          <div class="description">
            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Optio
            perferendis possimus laboriosam.
          </div>
          <div class="icon"><i class="fas fa-graduation-cap"></i></div>
        </div>
      </div>
      <div class="card staff">
        <div class="content">
          <div class="title">Excelência Profissional</div>
          <div class="description">
            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Optio
            perferendis possimus laboriosam.
          </div>
          <div class="icon"><i class="fa fa-chalkboard-teacher"></i></div>
        </div>
      </div>
      <div class="card management">
        <div class="content">
          <div class="title">Gestão Acolhedora</div>
          <div class="description">
            Lorem ipsum, dolor sit amet consectetur adipisicing elit. Optio
            perferendis possimus laboriosam.
          </div>
          <div class="icon"><i class="far fa-comments"></i></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Values",
};
</script>

<style scoped>
.values {
  margin: 6rem 0;
}

.values .cards {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
}

.cards .card {
  padding: 2rem;
  margin: 3rem 0;
  box-shadow: 0 0 8px 0 #5d524699;
  backface-visibility: hidden;
  -moz-backface-visibility: hidden;
  -webkit-backface-visibility: hidden;
  transition: all 0.2s;
}

.cards .card:hover {
  transform: translateY(-5px);
  box-shadow: 0 3px 8px 0 #5d5246cc;
}

.card .content {
  width: 50%;
  padding: 2rem;
  background: #ffffffef;
}

.cards .card.student {
  background: url("../../assets/images/student.jpg") center center / cover;
  /* Photo by <a href="https://unsplash.com/@linkedinsalesnavigator?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">LinkedIn Sales Solutions</a> on <a href="https://unsplash.com/s/photos/black-backpack?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>
   */
}

.cards .card.staff {
  background: url("../../assets/images/staff.jpg") center center / cover;
  /* Photo by <a href="https://unsplash.com/@wocintechchat?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Christina @ wocintechchat.com</a> on <a href="https://unsplash.com/s/photos/professional?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>
   */
}

.cards .card.management {
  background: url("../../assets/images/handshake.jpg") center left;
  /* Photo by <a href="https://unsplash.com/@cytonn_photography?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Cytonn Photography</a> on <a href="https://unsplash.com/s/photos/handshake?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>
   */
}

.card .icon {
  font-size: 4rem;
  margin-top: 1rem;
  color: #789d;
  text-align: right;
}

.card .title {
  text-transform: capitalize;
  font-variation-settings: "wght" 650;
  font-size: 1.8rem;
  margin-bottom: 1rem;
}

.card .description {
  font-size: 1.5rem;
  opacity: 0.9;
  /* padding: 1.6rem; */
}
</style>
