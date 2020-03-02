<template>
  <div class="gallery">
    <div>
      <section class="section_1">
        <div class="section_1_content">
          <p>LOOK AT US NOW!</p>
        </div>
      </section>

      <section class="section_2">
        <div class="section_2_content">
          <img src="../assets/images/gallery.png" />
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
  background: url(../assets/images/gallery-header.png);
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
.section_2 {
  padding: 100px 50px;
}
.section_2_content > img {
  display: block;
  margin: auto;
  width: 100%;
}
</style>