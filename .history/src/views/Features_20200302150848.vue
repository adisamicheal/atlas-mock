<template>
  <div class="features">
    <div>
      <section class="section_1">
        <div class="section_1_content">
          <p>FEATURES TO GIVE YOU A ROYAL EXPERIENCE</p>
        </div>
      </section>

      <section class="section_2">
        <div class="section_2_content">
          <img src="../assets/images/features/suite.png" />
          <img src="../assets/images/features/casino.png" />
          <img src="../assets/images/features/pool.png" />
          <img src="../assets/images/features/bar.png" />
          <img src="../assets/images/features/resturant.png" />
          <img src="../assets/images/features/conference-hall.png" />
          <img src="../assets/images/features/workspace.png" />
          <img src="../assets/images/features/gym.png" />
          <img src="../assets/images/features/room.png" />
        </div>
      </section>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.section_1 {
  background: url(../assets/images/features.png);
  height: 354px;
  background-size: cover;
  justify-content: center;
  align-items: center;
  display: flex;
}
.section_1_content {
  text-align: center;
}
.section_1_content p {
  font-family: Lato;
  font-style: normal;
  font-weight: 900;
  font-size: 34px;
  line-height: 41px;
  color: #ffffff;
  margin: 0;
}
.section_2_content {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-row-gap: 50px;
  grid-column-gap: 30px;
  justify-content: center;
  padding: 150px 50px;
}
.section_2_content > img {
  display: block;
  margin: auto;
  width: 100%;
}
/* */
/* .section_2_content>img::before {
	position: absolute;
	top: 0;
	left: -75%;
	z-index: 2;
	display: block;
	content: '';
	width: 50%;
	height: 100%;
	background: -webkit-linear-gradient(left, rgba(255,255,255,0) 0%, rgba(255,255,255,.3) 100%);
	background: linear-gradient(to right, rgba(255,255,255,0) 0%, rgba(255,255,255,.3) 100%);
	-webkit-transform: skewX(-25deg);
	transform: skewX(-25deg);
}
.section_2_content>img:hover::before {
	-webkit-animation: shine .75s;
	animation: shine .75s;
}
@-webkit-keyframes shine {
	100% {
		left: 125%;
	}
}
@keyframes shine {
	100% {
		left: 125%;
	}
} */
@media screen and (max-width: 1024px) {
  .section_2_content {
    grid-template-columns: 1fr 1fr;
  }
}

@media screen and (max-width: 768px) {
  .section_2_content {
    display: grid;
    grid-template-columns: 1fr;
    padding: 20px;
  }
}
</style>