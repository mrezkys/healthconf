<template>
    <div class="auth-page">
        <div class="container-lg">
            <Navbar/>
        </div>
        <div class="section-1">
            <div class="container-lg">
                <div class="col-xl-6 offset-xl-3 col-md-8 offset-md-2">
                    <img class="healthconfbox" src="~assets/icons/healthconfbox.svg" alt="">
                    <div class="auth-box">
                        <h3 class="header">Pilih cara masuk sebelum melakukan konsultasi</h3>
                        <div class="button-wrapper row">
                            <div class="col-6 pr-1">
                                <NuxtLink to="/login"><button class="btn btn-primary btn-lg">Masuk</button></NuxtLink>
                            </div>
                            <div class="col-6 pl-1">
                                <NuxtLink to="/register"><button class="btn btn-primary btn-lg">Daftar</button></NuxtLink>
                            </div>
                            <div class="col-12">
                                <NuxtLink to="/dashboard"><button class="btn btn-lg guest-button">Masuk Sebagai Tamu</button></NuxtLink>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>

 .healthconfbox{
     position: absolute;
     z-index: 2;
     top: -56px;
     right: -48px;
 }

 .auth-page{
    background-color: #07133A;
     min-height: 100vh;

    background-image: url(~assets/images/background-accent.png);
    background-size: cover;
    background-position: bottom;
 }

 .auth-page .section-1{
     padding: 80px 0;
 }

 .auth-page .section-1 .auth-box{
     background-color: white;
     border-radius: 20px;
     padding: 50px 50px 70px 50px;
 }

 .auth-page .section-1 .auth-box .header{
     font-family: 'Visby CF';
     font-weight: 800;
     font-size: 32px;
     line-height: 170%;
 }

.auth-page .section-1 .auth-box .button-wrapper{
    margin-top: 36px;
}

 .auth-page .section-1 .auth-box .button-wrapper .btn:hover{
     transform: scale(0.9);
     transition: 1s;
 }
 .auth-page .section-1 .auth-box .button-wrapper .btn{
     width: 100%;
     transition: 0.5s;
     padding-top: 20px;
     padding-bottom: 20px;
     font-size: 24px;
     font-family: 'Visby CF';
     font-weight: 600;
 }


 .auth-page .section-1 .auth-box .button-wrapper .guest-button{
     margin-top: 8px;
     background-color: #07133A;
     color: white;
 }

 /* TODO: make responisve for tablet because there is overflowed content */

  /* Mobile Responsive */
  @media (max-width: 575.98px) {
    .healthconfbox{
        display: none;
    }

    .auth-page{
        background-color: #07133A;
        min-height: 100vh;
        background-image: url(~assets/images/background-accent.png);
        background-size: cover;
        background-position: bottom;
    }

    .auth-page .section-1{
        padding: 40px 0;
    }

    .auth-page .section-1 .auth-box{
        background-color: white;
        border-radius: 20px;
        padding: 26px 26px 40px 26px;
    }

    .auth-page .section-1 .auth-box .header{
        font-size: 24px;
    }

    .auth-page .section-1 .auth-box .button-wrapper{
        margin-top: 24px;
    }

    .auth-page .section-1 .auth-box .button-wrapper .btn{
        font-size: 16px;
    }
  }

</style>