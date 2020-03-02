<template>
  <div class="about">
    <div>
      <section class="section_1">
        <div class="section_1_content">
          <p>OUR STORY</p>
        </div>
      </section>

      <section class="section_2">
        <div class="section_2_content">
          <div>
            <img src="../assets/images/about-image.png" />
          </div>
          <div class="grid_right">
            <h3>OUR VISION</h3>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
              incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis
              nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
              consequat.
            </p>
            <h3>OUR MISSION</h3>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
              incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis
              nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
              consequat.
            </p>
          </div>
        </div>
      </section>
    </div>
  </div>
</template>

<style scoped>
.section_1 {
  background: url(../assets/images/about-header.png);
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
  padding: 100px;
  display: grid;
  grid-template-columns: auto auto;
  grid-column-gap: 50px;
}
h3 {
  font-family: Lato;
  font-style: normal;
  font-weight: bold;
  font-size: 18px;
  line-height: 22px;
  color: #06122f;
}
.section_2_content p {
  font-family: Lato;
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 19px;
  color: #06122f;
}
.grid_right > h3:nth-child(3) {
  margin-top: 80px;
}
.section_2_content img {
  width: 100%;
}

@media (max-width: 768px) {
  .section_2_content {
    padding: 20px;
    display: grid;
    grid-template-columns: auto;
  }
  .section_2_content {
    display: block;
    width: 350px;
    margin: auto;
  }
}
</style>>
