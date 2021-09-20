<template>
    <div>
        <div class="footer">
            <div class="container-lg">
                <div class="row">
                <img class="logo pl-3" src="~assets/icons/logo.svg" alt="">
                <h3 class="company-name">Healthconf</h3>
                </div>
                <div class="row footer-content">
                <div class="col-md-5">
                    <p class="company-description">Healthconf adalah inisiatif para dokter yang menjadi relawan untuk memberi kontribusi ditengah pandemi melalui pemberian konsultasi gratis.</p>
                </div>
                <div class="offset-md-1 col-md-3">
                    <p class="company-info">No 40 Baria Sreet 133/2 Un Timur,Jakarta Barat, Indonesia.</p>
                    <p class="company-info">hi@healthconf.com</p>
                    <p class="company-info">(00) 123 456 789</p>
                </div>
                <div class="offset-md-1 col-md-2">
                    <h4 class="ikuti-kami">Ikuti Kami</h4>
                    <a href="https://instagram.com" target="_blank" class="company-info mt-2 d-block">Instagram</a>
                    <a href="https://fb.com" target="_blank" class="company-info mt-2 d-block">Facebook</a>
                    <a href="https://twitter.com" target="_blank" class="company-info mt-2 d-block">Twitter</a>
                </div>
                </div>
            </div>
        </div>
    </div>
</template>
<style scoped>

  .footer{
    background-color: #010425;
    padding-top: 60px;
    padding-bottom: 75px;
  }

  .footer .logo{
    height: 30px;
  }

  .footer .company-name{
    color: white;
      margin: 0 15px;
      font-family: 'Visby CF';
      font-weight: 700;
      font-size: 30px;
  }

  .footer .footer-content{
    margin-top: 32px;
  }

  .footer .footer-content .company-description{
    color: rgb(255, 255, 255, 80%);
    line-height: 180%;
    font-size: 20px;
  }

  .footer .footer-content .company-info{
    color: rgb(255, 255, 255, 60%);
  }

  .footer .footer-content .ikuti-kami{
    color: white;
    margin-top: 0;
    padding-top: 0;
    margin-bottom: 16px;
  }

  /* Mobile Responsive */

  
  @media (max-width: 575.98px) {

    .footer{
      background-color: #010425;
      padding-top: 40px;
      padding-bottom: 45px;
    }

    .footer .logo{
      height: 20px;
    }

    .footer .company-name{
      color: white;
       margin: 0 15px;
      font-size: 22px;
    }


    .footer .footer-content{
      margin-top: 16px;
    }

    .footer .footer-content .company-description{
      color: rgb(255, 255, 255, 80%);
      line-height: 180%;
      font-size: 16px;
    }

    .footer .footer-content .company-info{
      color: rgb(255, 255, 255, 60%);
    }

    .footer .footer-content .ikuti-kami{
      color: white;
      margin-top: 0;
      padding-top: 0;
      margin-bottom: 16px;
    }
  }
</style>