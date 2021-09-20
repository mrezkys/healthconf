<template>
    <div class="profile-page">
        <div class="container-lg">
            <DashboardNavbar/>
        </div>
        <div class="section-1">
            <div class="container-lg">
                <div class="col-xl-6 offset-xl-3 col-md-8 offset-md-2">
                    <img class="healthconfbox" src="~assets/icons/healthconfbox.svg" alt="">
                    <div class="form-box">
                        <h4 class="header">Informasi Akun</h4>
                        <form action="">
                            <input type="text" class="" placeholder="Nama Lengkap" value="mrezkys">
                            <input type="email" class="" placeholder="Alamat Email" value="emailkamu@email.com">
                            <div class="change-password">
                                <p class="subheader">Ganti kata sandi akun</p>
                                <input type="password" class="" placeholder="Kata Sandi Baru">
                                <input type="password" class="" placeholder="Konfirmasi Kata Sandi Baru">
                            </div>
                            <div class="row  submit-box">
                                <div class="col-6 my-auto">
                                    <NuxtLink to="/dashboard"><button class="btn btn-primary">Perbarui</button></NuxtLink>
                                </div>
                                <div class="col-6  pl-4 my-auto">
                                    <a href="/">Hapus akun saya</a>
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

    .profile-page{
        background-color: #07133A;
        min-height: 100vh;
        background-image: url(~assets/images/background-accent.png);
        background-size: cover;
        background-position: bottom;
    }


    .profile-page .section-1{
        padding: 80px 0;
    }

    .profile-page .section-1 .form-box{
        background-color: white;
        border-radius: 20px;
        padding: 50px 50px 70px 50px;
    }

    .profile-page .section-1 .form-box .header{
        font-family: 'Visby CF';
        font-weight: 800;
        font-size: 24px;
        line-height: 170%;
        margin: 0;
    }

    
    .profile-page .section-1 .form-box form input{
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

    .profile-page .section-1 .form-box form input:focus{
        border-radius: 20px;
        border: 1px solid #108AEE;
        outline: none;
    }

    .profile-page .section-1 .form-box form .change-password{
        margin-top: 40px;
    }

    .profile-page .section-1 .form-box form .change-password .subheader{
        margin: 0;
        margin-left: 12px;
        color: grey;
    }


    .profile-page .section-1 .form-box form .submit-box{
        margin-top: 40px;
    }

    .profile-page .section-1 .form-box form .submit-box button{
        padding-top: 20px;
        padding-bottom: 20px;
        width: 100%;
        border-radius: 10px;
        font-size: 22px;
        font-family: 'Visby CF';
        font-weight: 600;
    }

    .profile-page .section-1 .form-box form .submit-box a{
        font-size: 16px;
        color: grey;
        
    }


    /* TODO: make responisve for tablet because there is overflowed content */

    /* Mobile Responsive */
    @media (max-width: 575.98px) {
        .healthconfbox{
            display: none;
        }

        .profile-page{
            background-color: #07133A;
            min-height: 100vh;
            background-image: url(~assets/images/background-accent.png);
            background-size: cover;
            background-position: bottom;
        }

        .profile-page .section-1{
            padding: 40px 0;
        }

        .profile-page .section-1 .form-box{
            background-color: white;
            border-radius: 20px;
            padding: 26px 26px 40px 26px;
        }

        .profile-page .section-1 .form-box .change-password .subheader{
            font-size: 14px;
        }

        .profile-page .section-1 .form-box .header{
            font-size: 24px;
        }

        
        .profile-page .section-1 .form-box .header{
            font-size: 24px;
        }

        .profile-page .section-1 .form-box form input{
            width: 100%;
            margin-top: 16px;
            height: 50px;
            border-radius: 20px;
            border: none;
            background-color: rgb(159, 208, 249, 25%);
            font-size: 14px;
            padding-left: 30px;
        }

        .profile-page .section-1 .form-box form .submit-box button{
            font-size: 16px;
        }
        
        .profile-page .section-1 .form-box form .submit-box a{
            font-size: 14px;
        }
  }

</style>