<template>
    <div>
        <div class="navbar-wrapper">
            <div class="container-lg">
                <Navbar/> 
            </div>
        </div>
        <div class="section-1 ">
            <div class="container-lg">
                <div class="row">
                    <div class="col-md-5">
                        <h1 class="header">Ayo berkontribusi dengan menjadi Relawan.</h1>
                    </div>
                    <div class="offset-md-1 col-md-5 my-auto">
                        <p class="content">Kami membutuhkan bantuan relawan profesional untuk membantu lebih banyak orang lagi.</p>
                        <a href="#form"><button class="btn btn-primary">Daftar Sekarang</button></a>
                    </div>
                </div>
            </div>
        </div>
        <div class="section-2">
            <div class="container-lg">
                <h4 class="header">Alur Pendaftaran Relawan :</h4>
                <div class="row step-box-wrapper">
                <div class="col-md-3 step-box">
                    <h3 class="title">Daftar Online</h3>
                    <p class="subtitle">Kamu diharuskan mengisi formulir pendaftaran online dibawah, yang berisi data diri.</p>
                </div>
                <div class="col-md-3 step-box">
                    <h3 class="title">Seleksi Berkas</h3>
                    <p class="subtitle">Tahapan ini mengharuskan anda mengupload berkas berkas yang diperlukan.</p>
                </div>
                <div class="col-md-3 step-box">
                    <h3 class="title">Tes Wawancara</h3>
                    <p class="subtitle">Tes wawancara dilakukan setelah lulus tahapan seleksi berkas.</p>
                </div>
                <div class="col-md-3 step-box">
                    <h3 class="title">Pembekalan</h3>
                    <p class="subtitle">Setelah semuanya, sebelum menjadi relawan akan diberi pembekalan.</p>
                </div>
                </div>
            </div>
        </div>
        <div class="section-3" id="form">
            <div class="container-lg">
                <div class="col-md-7 p-1">
                    <h3 class="header">Formulir Pendaftaran Online Relawan</h3>
                    <p class="subheader">Kamu harus mengisi formulir dibawah ini dengan data diri yang sebenar benarnya dan berdasarkan diri sendiri.</p>
                </div>
                <div class="form">
                    <div class="row">
                        <div class="col-md-6">
                            <input type="text" class="" placeholder="Nama Lengkap">
                            <input type="text" class="" placeholder="Tanggal Lahir">
                        </div>
                        <div class="col-md-6">
                            <input type="text" class="" placeholder="Alamat">
                            <input type="text" class="" placeholder="Spesialisasi">
                        </div>
                        <div class="col-12">
                            <textarea placeholder="Ceritakan alasan anda mengapa ingin menjadi relawan disini..."></textarea>
                        </div>
                    </div>
                    <button class="btn btn-primary">Kirim Formulir</button>
                </div>
            </div>
        </div>
        <Footer/>
    </div>
</template>

<style scoped>
    .navbar-wrapper{
        background-color: #07133A;
    }

    .section-1{
        color: white;
        background-color: #07133A;
        background-image: url(~assets/images/background-accent.png);
        background-size: cover;
        background-position: bottom;
        background-repeat: no-repeat;
        padding-top: 56px;
        padding-bottom: 56px;
    }

    .section-1 .header{
        font-size: 50px;
        font-weight: 800;
        font-family: 'Visby CF';
        line-height: 150%;
    }

    .section-1 .content{
        font-size: 20px;
        line-height: 175%;
    }

    .section-1 .btn{
        padding: 16px 24px;
        font-size: 20px;
        font-family: 'Visby CF';
        border-radius: 10px;
        margin-top: 16px;
    }

    
  .section-2{
    background: #010425;
    padding: 45px 0px;
  }

  .section-2 .header{
    color: rgba(255, 255, 255, 0.3);
    font-weight: 600;
  }

  .section-2 .step-box-wrapper{
    margin-top: 32px;
  }

  .section-2 .step-box-wrapper .step-box{
    color: white;
  }

  .section-2 .step-box-wrapper .step-box .title{
    font-size: 26px;
    font-family: 'Visby CF';
    font-weight: 700;
    margin-bottom: 20px;
  }

  .section-2 .step-box-wrapper .step-box .subtitle{
    font-size: 16px;
    line-height: 175%;
    font-weight: 400;
    color: rgba(255, 255, 255, 0.8);
  }

  .section-3{
      padding-top: 52px;
      padding-bottom: 53px;
  }

  .section-3 .header{
    font-size: 32px;
    font-weight: 800;
    font-family: 'Visby CF';
    margin-bottom: 18px;
  }

    .section-3 .subheader{
        font-size: 18px;
        line-height: 175%;
    }


    .section-3 .form input{
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

    .section-3 .form input:focus{
        border-radius: 20px;
        border: 1px solid #108AEE;
        outline: none;
    }

    .section-3 .form textarea{
        width: 100%;
        margin-top: 24px;
        min-height: 150px;
        font-size: 18px;
        border-radius: 20px;
        border: none;
        background-color: rgb(159, 208, 249, 25%);
        font-size: 18px;
        padding: 30px;
    }

    .section-3 .form textarea:focus{
        border-radius: 20px;
        border: 1px solid #108AEE;
        outline: none;
    }

    .section-3 .form .btn{
        padding: 15px 30px;
        font-size: 18px;
        font-family: 'Visby CF';
        border-radius: 10px;
        margin-top: 24px;
    }

    @media (max-width: 1024px) {
        .section-1{
            padding-top: 26px;
        }
        .section-1 .header{
            font-size: 32px;
            margin-bottom: 16px;
        }

        .section-1 .content{
            font-size: 16px;
            margin-bottom: 8px;
        }

        .section-1 .btn{
            font-size: 16px;
            padding: 16px 24px;
            font-weight: 400;
        }


        .section-2 .header{
            color: rgba(255, 255, 255, 0.3);
            font-weight: 600;
            font-size: 20px;
        }

        .section-2 .step-box-wrapper{
            margin-top: 32px;
        }

        .section-2 .step-box-wrapper .step-box{
            color: white;
        }

        .section-2 .step-box-wrapper .step-box .title{
            font-size: 20px;
            margin-bottom: 16px;
        }

        .section-2 .step-box-wrapper .step-box .subtitle{
            font-size: 14px;
            line-height: 175%;
        }

        .section-3 .form input{
            font-size: 16px;
            padding: 16px;
        }

        .section-3 .form textarea{
            font-size: 16px;
            padding: 16px;
            line-height: 150%;
        }
    }

      /* Tablet */

</style>