<template>
    <div class="auth-page">
        <div class="container-lg">
            <Navbar/>
        </div>
        <div class="section-1">
            <div class="container-lg">
                <div class="col-xl-6 offset-xl-3 col-md-8 offset-md-2">
                    <img class="healthconfbox" src="~assets/icons/healthconfbox.svg" alt="">
                    <div class="form-box">
                        <h3 class="header">Halo, silahkan masuk untuk melanjutkan 😁</h3>
                        <form action="">
                            <input type="email" class="" placeholder="Alamat Email">
                            <input type="password" class="" placeholder="Kata Sandi">
                            <div class="row  submit-box">
                                <div class="col-6 my-auto">
                                    <NuxtLink to="/dashboard"><button class="btn btn-primary">Masuk</button></NuxtLink>
                                </div>
                                <div class="col-6 pl-2 my-auto">
                                    <NuxtLink to="/reset-password"><a>Lupa Kata Sandi? <strong class="text-primary">Atur Ulang</strong></a></NuxtLink>
                                </div>
                            </div>
                        </form>
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

 .auth-page .section-1 .form-box{
     background-color: white;
     border-radius: 20px;
     padding: 50px 50px 70px 50px;
 }

 .auth-page .section-1 .form-box .header{
     font-family: 'Visby CF';
     font-weight: 800;
     font-size: 32px;
     line-height: 170%;
 }

 .auth-page .section-1 .form-box form input{
     width: 100%;
     margin-top: 24px;
     height: 60px;
     font-size: 18px;
     border-radius: 20px;
     border: none;
     background-color: rgb(159, 208, 249, 25%);
     font-size: 18px;
     padding-left: 30px;
 }

 .auth-page .section-1 .form-box form input:focus{
     border-radius: 20px;
     border: 1px solid #108AEE;
     outline: none;
 }

 .auth-page .section-1 .form-box form .submit-box{
     margin-top: 40px;
 }

 .auth-page .section-1 .form-box form .submit-box button{
     padding-top: 20px;
     padding-bottom: 20px;
     width: 100%;
     border-radius: 10px;
     font-size: 22px;
     font-family: 'Visby CF';
     font-weight: 600;
 }

 .auth-page .section-1 .form-box form .submit-box a{
     font-size: 14px;
     color: grey;
     
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

    .auth-page .section-1 .form-box{
        background-color: white;
        border-radius: 20px;
        padding: 26px 26px 40px 26px;
    }

    .auth-page .section-1 .form-box .header{
        font-size: 24px;
    }

    .auth-page .section-1 .form-box form input{
        width: 100%;
        margin-top: 16px;
        height: 50px;
        border-radius: 20px;
        border: none;
        background-color: rgb(159, 208, 249, 25%);
        font-size: 14px;
        padding-left: 30px;
    }

    .auth-page .section-1 .form-box form .submit-box button{
        font-size: 16px;
    }
  }

</style>