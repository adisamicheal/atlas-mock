<template>
  <div class="footer">
      <div class="footer_content">
        <div>
            <p>Atlas Hotels</p>
            <p><a href="tel:+2349091271976">+234 80795637</a></p> 
            <p><a href="mailto:adisamicheal20@gmail.com">hotel@atlas.money</a></p>
        </div>
        <div class="icons">
            <div class="icon-images">
                <img src="../assets/icon/person-icon.svg">
                <a href="tel:+2349091271976"><img src="../assets/icon/call.svg"></a>
                <a href="mailto:adisamicheal20@gmail.com"><img src="../assets/icon/message.svg"></a>
            </div>
            <div class="logo-footer">
                <img src="../assets/icon/atlas.svg">
                <p>Atlas</p>
            </div>
        </div>
        <div>
            <p>No. 9 Latinos Street,</p> <p>Ajebo Road Abuja</p>
        </div>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.footer{
    background: #06122F;
    color: #ffffff;
    padding: 50px 200px;
    /* margin-top: 100px; */
}
.footer_content{
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
}
.icons{
    text-align: center;
}
.icon-images{
    display: flex;
    justify-content: space-around;
    padding: 0 100px;
    margin-top: 70px;
}
.logo-footer{
    margin-top: 50px;
}
p{
    font-family: Lato;
    font-style: normal;
    font-weight: bold;
    font-size: 14px;
    line-height: 18px;
    margin: 0;
    margin-top: 10px;
    text-align: center;
}
a{
    text-decoration: none;
    color: #ffffff;
}

@media (max-width: 768px){
    .footer{
        padding: 0;
    }
    .footer_content{
        display: grid;
        grid-template-columns: 1fr;
        padding: 20px 0;
    }
}
</style>>
