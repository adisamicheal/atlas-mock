<template>
  <div class="contact">
    <div>
      <section class="section_1">
        <div class="section_1_content">
          <p>Get in Touch</p>
        </div>
        <div>
          <img src="../assets/icon/location.png" class="location" />
        </div>
      </section>

      <section class="section_2">
        <div class="section_2_content">
          <div class="form">
            <div class="form-content">
              <div class="form-heading">
                <p>Send Us a Message</p>
                <img src="../assets/icon/mail.svg" />
              </div>
              <div class="form-group-container">
                <div class="form-group">
                  <label for="name">Your Name</label>
                  <input type="text" />
                </div>
                <div class="form-group">
                  <label for="name">Email Address</label>
                  <input type="email" />
                </div>
                <div class="form-group">
                  <label for="name">Mobile Number</label>
                  <input type="tel" />
                </div>
                <div class="form-group">
                  <label for="name">Company</label>
                  <input type="text" />
                </div>
                <div class="form-group">
                  <label for="name">Message</label>
                  <input type="text" />
                </div>
              </div>
              <div class="form-footer">
                <img src="../assets/icon/send-message.svg" />
              </div>
            </div>
          </div>
          <div class="address">
            <div class="address-content">
              <p>Contact Information</p>
              <div class="content-body">
                <img src="../assets/icon/location-small.png" />
                <p>
                  Atlas Money Ghana Ltd, Graphic Road, Accra
                  GA-216, 2665 Graphic Rd, Accra, Ghana
                </p>
              </div>
              <div class="content-body">
                <img src="../assets/icon/mail-small.png" />
                <p>support@atlas.money</p>
              </div>
              <div class="content-body">
                <img src="../assets/icon/phone.png" />
                <p>+231 621-540-987</p>
              </div>
              <div class="socials">
                <img src="../assets/icon/twitter.png" />
                <img src="../assets/icon/instagram.png" />
                <img src="../assets/icon/linkedin.png" />
              </div>
            </div>
          </div>
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
  background: url(../assets/images/contact-header.png);
  height: 502.27px;
  background-size: cover;
}
.section_1_content {
  padding: 200px 0 0 0;
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
.location {
  display: block;
  margin: auto;
  padding-left: 700px;
  padding-top: 50px;
}
.section_2_content {
  display: flex;
  justify-content: center;
  padding: 150px;
}
.form {
  background: #ffffff;
  box-shadow: 0px 20px 30px rgba(0, 0, 0, 0.25);
  padding: 50px;
}
.form-group-container {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-row-gap: 30px;
  grid-column-gap: 50px;
  margin-top: 50px;
}
.form-heading {
  display: flex;
  justify-content: space-between;
  font-family: Lato;
  font-style: normal;
  font-weight: bold;
  font-size: 24px;
  line-height: 29px;
  color: #06122f;
}
.form-group > input {
  outline: none;
  border: none;
  border-bottom: 1px solid #000000;
}
.form-group > input,
label {
  display: block;
  width: 300px;
}
label {
  font-family: Lato;
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 19px;
  color: #06122f;
  margin-bottom: 30px;
}
.form-footer > img {
  margin-top: 30px;
  float: right;
}
.address {
  background: #06122f;
  box-shadow: 0px 30px 20px rgba(0, 0, 0, 0.25);
  padding: 0 50px;
}
.address-content > p {
  font-family: Lato;
  font-style: normal;
  font-weight: normal;
  font-size: 24px;
  line-height: 29px;
  color: #ffffff;
}
.content-body > p {
  font-family: Lato;
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  line-height: 17px;
  color: #ffffff;
}
.content-body > img {
  display: block;
  margin: auto auto auto 0;
}
.content-body {
  display: grid;
  grid-template-columns: 0.3fr 1fr;
  margin-top: 45px;
}
.socials {
  display: flex;
  justify-content: space-between;
  margin-top: 50px;
}

@media (max-width: 1024px) {
  .section_2_content {
    flex-direction: column;
    padding: 30px 0;
  }
  .form-group-container {
    grid-template-columns: 1fr;
  }
}
@media (max-width: 768px) {
  .section_2_content {
    flex-direction: column;
    padding: 30px 0;
  }
  .form-group-container {
    grid-template-columns: 1fr;
  }
}
</style>