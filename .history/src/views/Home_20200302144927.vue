<template>
  <div class="home">
    <div style="background: #F4F4F1;">
      <section class="section_1">
        <div class="section_1_content">
          <span class="wel">Welcome!</span>
          <span class="come">
            TO THE
            <br />HOME OF YOUR DREAMS
          </span>
        </div>
      </section>
      <div class="form-container">
        <form>
          <input type="search" placeholder="Type your Room" />
          <input type="date" />
          <input type="date" />
          <button>BOOK NOW</button>
        </form>
      </div>

      <section class="section_2">
        <div class="section_2_content">
          <div>
            <img src="../assets/images/beach-side.png" />
          </div>
          <div class="bg__white">
            <div class="bg__white__content">
              <h3>WHY ATLAS</h3>
              <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                Curabitur cursus tellus nec justo rutrum gravida vel eu nisl.
                Praesent tinciduntellus. Proin sit amet vehicula nulla. Maecenas
                sollicitudin ullamcorper justo. Praesent
              </p>
              <p>
                It is a long established fact that a reader will
                be distracted by the readable content of a page when looking
                at its layout. The point of using Lorem Ipsum.There are many
                variations of passages of Lorem Ipsum available, but the majority
                have suffered alteration in some form, by injected humour, or
                randomised words which don't look even slightly believable.
              </p>
              <button>BOOK NOW</button>
            </div>
          </div>
        </div>
      </section>

      <section class="section_3">
        <div>
          <h3>OUR ROOMS</h3>
          <div class="h3-div"></div>
          <p>View all our rooms</p>
        </div>
        <div>
          <vueper-slides
            class="no-shadow"
            :visible-slides="4"
            slide-multiple
            :gap="3"
            :slide-ratio="1 / 4"
            :dragging-distance="200"
            :breakpoints="{ 800: { visibleSlides: 2, slideMultiple: 2 } }"
          >
            <vueper-slide
              v-for="(slide, i) in slides"
              :key="i"
              :image="slide.image"
              :title="slide.title"
              :content="slide.content"
              :link="slide.link"
            />
          </vueper-slides>
        </div>
      </section>

      <section class="section_4">
        <div class="section_4_content">
          <h3>CUSTOMER REVIEWS</h3>
          <div></div>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit.
            Curabitur cursus tellus nec justo rutrum gravida vel eu nisl.
            Praesent tincidunt ultricies pulvinar. Nullam sit amet mi pharetra,
            facilisis lacus a, condimentum eros. Maecenas ut tincidunt tellus.
            Proin sit amet vehicula nulla. Maecenas sollicitudin ullamcorper justo.
            Praesent et porttitor turpis.
          </p>
          <p>- Somto Onyekwere</p>
        </div>
      </section>

      <section class="section_5">
        <div class="section_5_content">
          <h3>OUR PROCESS</h3>
          <div class="h3-div"></div>
          <p>Our process is fast and easy and can be done from anywhere in the world anytime</p>
          <div class="bg__navy__parent">
            <div class="bg__navy">
              <img src="../assets/icon/contact.svg" />
              <p>You fill in the booking form to make a reservation</p>
            </div>
            <div class="bg__navy">
              <img src="../assets/icon/card.svg" />
              <p>You fill in the booking form to make a reservation</p>
            </div>
            <div class="bg__navy">
              <img src="../assets/icon/telegram.svg" />
              <p>You fill in the booking form to make a reservation</p>
            </div>
          </div>
        </div>
      </section>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import { VueperSlides, VueperSlide } from "vueperslides";
import "vueperslides/dist/vueperslides.css";

export default {
  name: "Home",
  components: {
    VueperSlides,
    VueperSlide
  },
  data: () => ({
    slides: [
      {
        image: require("../assets/images/room1.png")
      },
      {
        image: require("../assets/images/room2.png")
      },
      {
        image: require("../assets/images/room3.png")
      },
      {
        image: require("../assets/images/room4.png")
      },
      {
        image: require("../assets/images/room1.png")
      },
      {
        image: require("../assets/images/room2.png")
      },
      {
        image: require("../assets/images/room3.png")
      },
      {
        image: require("../assets/images/room4.png")
      },
      {
        image: require("../assets/images/room1.png")
      },
      {
        image: require("../assets/images/room2.png")
      },
      {
        image: require("../assets/images/room3.png")
      },
      {
        image: require("../assets/images/room4.png")
      },
      {
        image: require("../assets/images/room1.png")
      },
      {
        image: require("../assets/images/room2.png")
      },
      {
        image: require("../assets/images/room3.png")
      },
      {
        image: require("../assets/images/room4.png")
      }
      // Other slides.
    ]
  })
};
</script>

<style scoped>
/* body{
  background: #F4F4F1;
} */
.section_1 {
  background: url(../assets/images/home.png);
  height: 700px;
}
.section_1_content {
  padding: 200px 400px 200px 150px;
}
.section_1 .wel {
  font-family: Xtreem Medium;
  font-size: 127px;
  line-height: 186px;
  color: #ffffff;
}
.section_1 .come {
  margin-left: 30px;
  font-family: Roboto;
  font-size: 70px;
  line-height: 56px;
  font-weight: 700px;
  color: #ffffff;
}
.form-container {
  width: 80%;
  /* height: 136px; */
  background: #ffffff;
  box-shadow: 0px 5px 6px rgba(0, 0, 0, 0.2);
  display: block;
  margin: auto;
  /* margin-top: -65px;
  position: absolute; */
  transform: translateY(-50%);
}
.form-container > form {
  display: flex;
  justify-content: space-between;
  padding: 50px 70px;
}
input[type="search"] {
  width: 40%;
  height: 47px;
  background: #ffffff;
  border: 1px solid #979797;
}
input[type="date"] {
  width: 20%;
  height: 47px;
  background: #ffffff;
  border: 1px solid #979797;
}
button {
  width: 12%;
  height: 41px;
  background: #06122f;
  font-family: Roboto, "san-serif";
  font-style: normal;
  font-weight: bold;
  font-size: 14px;
  line-height: 16px;
  color: #ffffff;
  outline: none;
  cursor: pointer;
}

.section_2 {
  /* height: 740px; */
  background: #f4f4f1;
}
.section_2_content {
  padding: 10px 115px 0 115px;
  display: flex;
}
.section_2_content h3 {
  font-family: "Lato", sans-serif;
  font-style: normal;
  font-weight: bold;
  font-size: 18px;
  line-height: 22px;
  color: #06122f;
}
.section_2_content p {
  font-family: "Lato", sans-serif;
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  line-height: 25px;
  color: #000000;
}
.section_2_content button {
  width: 25%;
  margin-top: 50px;
}
.bg__white {
  height: 510px;
  background: #ffffff;
}
.bg__white__content {
  padding: 0 20px;
}

.section_3 {
  background: #06122f;
  text-align: center;
}
.section_3 h3 {
  font-family: Roboto;
  font-style: normal;
  font-weight: bold;
  font-size: 18px;
  line-height: 21px;
  color: #ffffff;
  margin: 0;
  padding: 15px 0 10px 0;
}
.h3-div {
  width: 40px;
  border-bottom: 2px solid white;
  display: block;
  margin: auto;
}
.section_3 p {
  font-family: Roboto;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 19px;
  color: #ffffff;
  margin: 0;
  margin-top: 10px;
}

.section_4 {
  text-align: center;
  height: 392px;
  background: url(../assets/images/pool-side.png);
}
.section_4_content {
  padding: 50px 150px;
}
.section_4_content h3:nth-child(1) {
  font-family: Lato;
  font-style: normal;
  font-weight: bold;
  font-size: 18px;
  line-height: 32px;
  color: #ffffff;
  margin: 0;
}
.section_4_content div:nth-child(2) {
  width: 80px;
  border-bottom: 2px solid white;
  display: block;
  margin: auto;
  margin-top: 10px;
}
.section_4_content > p:nth-child(3) {
  font-family: Lato;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 29px;
  text-align: center;
  color: #ffffff;
  margin-top: 60px;
}
.section_4_content > p:nth-child(4) {
  font-family: Roboto;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 19px;
  color: #ffffff;
  margin-top: 60px;
}

.section_5 {
  text-align: center;
  /* height: 734px; */
  background: #f4f4f1;
}
.section_5_content > h3:nth-child(1) {
  font-family: Roboto;
  font-style: normal;
  font-weight: bold;
  font-size: 18px;
  line-height: 32px;
  color: #06122f;
  margin: 0;
  margin-top: 30px;
}
.section_5_content > div:nth-child(2) {
  width: 80px;
  border-bottom: 2px solid #2e1b4c;
  display: block;
  margin: auto;
  margin-top: 10px;
}
.section_5_content p:nth-child(3) {
  font-family: Lato;
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 29px;
  text-align: center;
  color: #000000;
  margin-top: 50px;
}
.bg__navy__parent {
  padding: 100px;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-column-gap: 40px;
  padding: 30px 150px;
}
.bg__navy {
  /* width: 100%; */
  background: #06122f;
  text-align: center;
  padding: 120px 50px;
}
.bg__navy > p {
  font-family: Lato;
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  line-height: 17px;
  text-align: center;
  color: #ffffff;
}

@media (max-width: 768px) {
  .section_1 {
    height: 400px;
  }
  .section_1_content {
    text-align: center;
    padding: 100px;
  }
  .section_1 .wel {
    font-family: Xtreem Medium;
    font-size: 50px;
    line-height: 56px;
    color: #ffffff;
  }
  .section_1 .come {
    margin-left: 30px;
    font-family: Roboto;
    font-size: 30px;
    line-height: 56px;
    font-weight: 700px;
    color: #ffffff;
  }
  input[type="search"] {
    width: 25%;
  }
  input[type="date"] {
    width: 25%;
  }
  button {
    width: 15%;
  }
  .section_2 img {
    width: 400px;
  }
  .section_2_content {
    display: flex;
    flex-direction: column;
    padding: 10px;
  }
  .form-container {
    width: 100%;
  }
  .form-container > form {
    padding: 10px 10px;
  }
  .section_4_content {
    padding: 1px 10px;
  }
  .bg__navy__parent {
    margin-top: 0;
    display: grid;
    grid-template-columns: 1fr;
    grid-row-gap: 40px;
    padding: 10px;
  }
}
</style>

<style>
.vueperslides {
  padding: 30px 300px;
}
.vueperslide__title,
.vueperslide__content {
  color: white;
}
.vueperslides__arrow svg {
  fill: white;
}
.vueperslides__arrows--outside .vueperslides__arrow--next {
  right: -3.5em;
}
@media (max-width: 768px) {
  .vueperslides {
    padding: 5px;
  }
  .vueperslides__arrows--outside .vueperslides__arrow--next {
    right: -0.5em;
  }
}
</style>
