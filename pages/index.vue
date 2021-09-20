<template>
  <div>
    <div class="section-1">
      <div class="container-lg">
        <Navbar/> 
      </div>
      <div class="container-lg mt-4">
        <div class="row">
          <div class="col-md-6 welcome-box my-auto">
            <h1 class="welcome-title">
              Konsultasi covid <span style="font-weight: 800">&</span> mental dengan kami.
            </h1>
            <h4 class="welcome-subtitle">
              Konsultasi seputar covid dan mental health secara gratis dengan dokter yang spesialis dibidangnya.
            </h4>
            <div class="row">
              <NuxtLink to="/auth">
                <button class="btn btn-primary konsultasi-button">Konsultasi Sekarang</button>
              </NuxtLink>
              <NuxtLink to="#panduan">
              <button class="btn btn-outline-light panduan-button">Panduan 
                <svg  class="bottom-icon" width="32" height="32" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <path fill-rule="evenodd" clip-rule="evenodd" d="M10.2212 28.3333H21.7798C25.8065 28.3333 28.3332 25.4813 28.3332 21.4453V10.5547C28.3332 6.51867 25.8198 3.66667 21.7798 3.66667H10.2212C6.18117 3.66667 3.6665 6.51867 3.6665 10.5547V21.4453C3.6665 25.4813 6.18117 28.3333 10.2212 28.3333Z" stroke="white" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
                  <path d="M15.9997 21.448V10.552" stroke="white" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
                  <path d="M20.9971 16.4297L15.9998 21.4484L11.0024 16.4297" stroke="white" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
                </svg>
              </button>
              </NuxtLink>
            </div>
          </div>
          <div class="col-md-6 welcome-image-box">
            <img class="img-fluid welcome-image" src="~assets/images/conference.png" alt="">
          </div>
        </div>
      </div>
    </div>
    <div class="section-2" id="panduan">
      <div class="container-lg">
        <h4 class="header">4 Langkah Mudah</h4>
        <div class="row step-box-wrapper">
          <div class="col-md-3 step-box">
            <h3 class="title">Daftar akun</h3>
            <p class="subtitle">Kamu bisa mendaftarkan akun dengan mengklik tombol Konsultasikan Sekarang.</p>
          </div>
          <div class="col-md-3 step-box">
            <h3 class="title">Pilih Layanan</h3>
            <p class="subtitle">Langkah selanjutnya adalah memilih layanan konsultasi melalui chat atau video call.</p>
          </div>
          <div class="col-md-3 step-box">
            <h3 class="title">Jadwalkan</h3>
            <p class="subtitle">Jadwalkan konsultasi anda dengan dokter agar bisa menyesuaikan waktu anda.</p>
          </div>
          <div class="col-md-3 step-box">
            <h3 class="title">Konsultasikan</h3>
            <p class="subtitle">Saat tiba giliran anda, anda dapat mengkonsultasikan masalah yang anda alami.</p>
          </div>
        </div>
        <div class="row help-box">
          <div class="col-md-6 my-auto">
            <h4 class="help-text">Masih belum jelas? silahkan melihat :</h4>
          </div>
          <div class="col-md-3 col-6">
            <a href="https://youtube.com" target="_blank"><button class="btn btn-outline-light btn-lg help-button">Video Panduan</button></a>
          </div>
          <div class="col-md-3 col-6">
            <a href="https://drive.google.com" target="_blank"><button class="btn btn-outline-light btn-lg help-button">Pdf Panduan</button></a>
          </div>
        </div>
      </div>
    </div>
    <div class="section-3">
      <div class="container-lg">
        <div class="row">
          <div class="col-md-6 info-box my-auto">
            <h1 class="title">Konsultasi kesehatan gratis secara Virtual.</h1>
            <h4 class="subtitle">Kamu bisa menkonsultasikan tentang kesehatan di masa pandemi seperti tentang Covid19 atau tentang Kesehatan Mental secara virtual dengan layanan chat atau video call.</h4>
          </div>
          <div class="col-md-6 info-image">
            <img class="img-fluid" src="~assets/images/elis.png" alt="">
          </div>
        </div>
        <div class="row info">
          <div class="col-md-6 detail-info-wrapper">
            <div class="col-12">
              <div class="row">
                <div class="icon-box d-flex align-items-center justify-content-center">
                  <img class="" src="~assets/icons/videocall.svg" alt="">
                </div>
                <div class="detail-info-box col-md-8 col-9 my-auto">
                  <h3 class="title">Konsultasi Covid & Mental melalui Video Call</h3>
                  <p class="subtitle">Konsultasi seputar covid dan mental health secara gratis.</p>
                </div>
              </div>
            </div>
          </div>
          <div class="col-md-6 detail-info-wrapper">
            <div class="col-12">
              <div class="row">
                <div class="icon-box d-flex align-items-center justify-content-center">
                  <img class="" src="~assets/icons/chat.svg" alt="">
                </div>
                <div class="detail-info-box col-md-8 col-9 my-auto">
                  <h3 class="title">Konsultasi Covid & Mental melalui Chat</h3>
                  <p class="subtitle">Konsultasi seputar covid dan mental health secara gratis.</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="section-4">
      <div class="container-lg">
        <div class="row">
          <div class="col-md-6">
            <h1 class="header">Relawan Profesional yang siap membantu.</h1>
          </div>
          <div class="col-md-6 my-auto">
            <h4 class="subheader">Jangan ragu untuk berkonsultasi. Di Healtconf para relawan merupakan Dokter yang Profesional di Bidangnya.</h4>
          </div>
        </div>
        <div class="row doctor-wrapper">
          <div class="col-md-3 col-6 text-center doctor-box">
            <img class="doctor-avatar" src="~assets/images/elissiamyla.png" alt="">
            <h4 class="doctor-name">Elissia Myla</h4>
            <p class="doctor-title">Psikiater</p>
          </div>
          <div class="col-md-3 col-6 text-center doctor-box">
            <img class="doctor-avatar" src="~assets/images/karen.png" alt="">
            <h4 class="doctor-name">Karen Agnola</h4>
            <p class="doctor-title">Psikolog</p>
          </div>
          <div class="col-md-3 col-6 text-center doctor-box">
            <img class="doctor-avatar" src="~assets/images/elizza.png" alt="">
            <h4 class="doctor-name">Elissia Myla</h4>
            <p class="doctor-title">Psikiater</p>
          </div>
          <div class="col-md-3 col-6 text-center doctor-box">
            <img class="doctor-avatar" src="~assets/images/jessyca.png" alt="">
            <h4 class="doctor-name">Jessyca Mi</h4>
            <p class="doctor-title">Dokter</p>
          </div>
          <div class="col-md-3 col-6 text-center doctor-box">
            <img class="doctor-avatar" src="~assets/images/hena.png" alt="">
            <h4 class="doctor-name">Hena Syafira</h4>
            <p class="doctor-title">Psikiater</p>
          </div>
          <div class="col-md-3 col-6 text-center doctor-box">
            <img class="doctor-avatar" src="~assets/images/nora.png" alt="">
            <h4 class="doctor-name">Elissia Myla</h4>
            <p class="doctor-title">Psikiater</p>
          </div>
          <div class="col-md-3 col-6 text-center doctor-box">
            <img class="doctor-avatar" src="~assets/images/jeremy.png" alt="">
            <h4 class="doctor-name">Jeremy Alam</h4>
            <p class="doctor-title">Psikolog</p>
          </div>
          <div class="col-md-3 col-6 text-center join-box">
            <img class="join-icon" src="~assets/icons/addmember.svg" alt="">
              <NuxtLink to="/relawan" style="text-decoration: none; color: black">
              <h4 class="join-title">Gabung Menjadi Relawan
                <svg width="29" height="29" viewBox="0 0 29 29" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <path d="M23.8647 14.1685L5.73975 14.1685" stroke="#071238" stroke-width="3.5" stroke-linecap="round" stroke-linejoin="round"/>
                  <path d="M16.5547 6.88903L23.8651 14.168L16.5547 21.4482" stroke="#071238" stroke-width="3.5" stroke-linecap="round" stroke-linejoin="round"/>
                </svg>
              </h4>
              </NuxtLink>
          </div>
        </div>
      </div>
    </div>
    <div class="section-5">
      <div class="container-lg">
        <div class="row">
          <div class="col-md-4 my-auto">
            <h3 class="title">Berkontribusi dengan menjadi Relawan.</h3>
          </div>
          <div class="col-md-4 my-auto">
            <p class="subtitle">Kami membutuhkan bantuan relawan profesional untuk membantu lebih banyak orang lagi.</p>
          </div>
          <div class="col-md-4 my-auto d-flex justify-content-end button-wrapper">
            <NuxtLink to="/relawan"><button class="button btn">Daftar Sekarang <img class="ml-2" src="~assets/icons/ArrowRight.svg" alt=""></button></NuxtLink>
          </div>
        </div>
      </div>
    </div>
    <Footer/>
  </div>
</template>

<style scoped>
  .section-1{
    background-color: #07133A;
    min-height: 684px;
    background-image: url(~assets/images/background-accent.png);
    background-size: contain;
  }

  .section-1 .welcome-box .welcome-title{
    color: white;
    font-size: 46px;
    font-weight: 800;
    line-height: 150%;
    margin-bottom: 24px;
    font-family: 'Visby CF';
  }

  .section-1 .welcome-box .welcome-subtitle{
    color: white;
    filter: opacity(0.8);
    font-size: 22px;
    line-height: 175%;
    font-weight: 400;
    width: 85%;
    margin-bottom: 50px;
  }

  .section-1 .welcome-box .btn{
    margin-left: 16px;
    padding: 20px 30px;
    font-size: 24px;
    border-radius: 10px;
    font-family: 'Poppins';
    font-weight: 400;
  }

  .section-1 .welcome-box .panduan-button{
    border: 1px solid rgba(255, 255, 255, 0.5);
    color: rgba(255, 255, 255, 0.5);

  }

  .section-1 .welcome-box .konsultasi-button{
  }

  .section-1 .welcome-box .panduan-button:hover{
    background: none;
    border: 1px solid white;
    color: white;
  }

  .section-1 .welcome-box .panduan-button .bottom-icon{
    margin-left: 8px;
  }

  .section-1 .welcome-image-box{
    padding-left: 48px;
  }

  .section-2{
    background: #010425;
    min-height: 385px;
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

  .section-2 .help-box{
    margin-top: 48px;
  }

  .section-2 .help-box .help-button{
    color: rgba(255, 255, 255, 0.7);
    font-size: 18px;
    border: 1px solid rgba(255, 255, 255, 0.4);
    border-radius: 5px;
  }

  .section-2 .help-box .help-button:hover{
    color: #010425;
  }


  .section-2 .help-box .help-text{
    color: white;
    font-size: 22px;
    font-weight: 500;
  }

  .section-3{
    padding-top: 20px;
    padding-bottom: 100px;
  }

  .section-3 .info{
    margin-top: 60px;
  }


  .section-3 .info-box .title{
    color: black;
    font-size: 46px;
    font-weight: 800;
    line-height: 150%;
    margin-bottom: 24px;
    margin-top: 56px;
    font-family: 'Visby CF';
  }

  .section-3 .info-box .subtitle{
    color: black;
    filter: opacity(0.8);
    font-size: 22px;
    line-height: 175%;
    font-weight: 400;
  }

  .section-3 .info-image{
  }

  .section-3 .detail-info-wrapper .icon-box{
    width: 180px;
    height: 180px;
    border-radius: 20px;
    background-color: rgb(159, 208, 249, 40%);
  }

  .section-3 .detail-info-wrapper .detail-info-box{
    padding-left: 32px;
  }

  .section-3 .detail-info-wrapper .detail-info-box  .title{
    font-size: 26px;
    font-family: 'Visby CF';
    font-weight: 800;
    line-height: 150%;
    margin-bottom: 16px;
  }

  .section-3 .detail-info-wrapper .detail-info-box  .subtitle{
    font-size: 16px;
    line-height: 175%;
    margin: 0;
  }

  .section-4{
    padding-top: 60px;
    margin-bottom: 80px;
  }

  .section-4 .header{
    color: black;
    font-size: 46px;
    font-weight: 800;
    line-height: 150%;
    font-family: 'Visby CF';
  }

  .section-4 .subheader{
    color: black;
    filter: opacity(0.8);
    font-size: 22px;
    line-height: 175%;
    font-weight: 400;
  }

  .section-4 .doctor-wrapper{
    margin-top: 36px;
  }

  .section-4 .doctor-wrapper .doctor-box{
    margin-top: 32px;
  }
  .section-4 .doctor-wrapper .doctor-box .doctor-avatar{
    margin-bottom: 16px;
  }

  .section-4 .doctor-wrapper .doctor-box .doctor-name{
    font-size: 26px;
    font-weight: 600;
  }

  .section-4 .doctor-wrapper .join-box{
    margin-top: 32px;
  }


  .section-4 .doctor-wrapper .join-box .join-icon{
    margin-bottom: 16px;
  }

  .section-4 .doctor-wrapper .join-box  .join-title{
    font-size: 24px;
    font-weight: 600;
    line-height: 150%;
    text-align: center !important;
  }



  .section-5{
    padding: 72px 0px;
    background-color: #108AEE;
  }

  .section-5 .title{
    color: white;
    font-size: 32px;
    font-weight: 800;
    line-height: 150%;
    font-family: 'Visby CF';
    padding: 0;
    margin: 0;
  }

  .section-5 .subtitle{
    color: rgb(255, 255, 255, 80%);
    padding: 0;
    margin: 0;
  }

  .section-5 .button-wrapper  .button{
    padding: 30px;
    color: white;
    background-color: #010425;
    font-size: 24px;
    font-weight: 600;
    border-radius: 20px;
    transition: 0.5s;
  }

  .section-5 .button-wrapper .button:hover{
    transform: scale(1.1);
    transition: 1s;
  }



  /* Mobile Responsive */

  
  @media (max-width: 1024px) {
    .section-1{
      background-size: cover;
      min-height: 500px;
    }

    .section-1 .welcome-box .welcome-title{
      color: white;
      font-size: 32px;
      margin-bottom: 16px;
    }

    .section-1 .welcome-box .welcome-subtitle{
      color: white;
      font-size: 16px;
      margin-bottom: 32px;
    }


    .section-1 .welcome-box .row .btn{
      margin-left: 16px;
      padding: 10px 15px !important;
      font-size: 14px;
      border-radius: 10px;
      font-family: 'Poppins';
      font-weight: 400;
    }
    

    .section-1 .welcome-image-box{
      padding: 16px;
      margin: 24px 0;
    }

    .section-2 .step-box-wrapper .step-box .title{
      font-size: 20px;
      margin-bottom: 16px;
    }

    .section-2 .step-box-wrapper .step-box .subtitle{
      font-size: 14px;
      line-height: 175%;
    }

    .section-2 .help-box{
      margin-top: 32px;
    }

    .section-2 .help-box .help-button{
      font-size: 16px;
      border-radius: 5px;
    }

    .section-2 .help-box .help-text{
      color: white;
      font-size: 16px;
      font-weight: 500;
      margin-bottom: 18px;
    }

    .section-3{
      padding-bottom: 16px;
    }

    .section-3 .info-box .title{
      color: black;
      font-size: 32px;
      margin-bottom: 16px;
      margin-top: 32px;
    }

    .section-3 .info-box .subtitle{
      color: black;
      filter: opacity(0.8);
      font-size: 16px;
      line-height: 175%;
      font-weight: 400;
    }

    .section-3 .info-image{
    }

    .section-3 .detail-info-wrapper{
      margin-top: 24px;
    }

    .section-3 .detail-info-wrapper .icon-box{
      width: 80px;
      height:80px;
      padding: 24px;
      border-radius: 20px;
      background-color: rgb(159, 208, 249, 40%);
    }

    .section-3 .info{
      margin-top: 8px;
    }
    .section-3 .detail-info-wrapper .icon-box img{
      width: 48px;
    }

    .section-3 .detail-info-wrapper .detail-info-box{
      padding-left: 16px;
    }

    .section-3 .detail-info-wrapper .detail-info-box  .title{
      font-size: 19px;
      font-family: 'Visby CF';
      font-weight: 700;
      line-height: 150%;
      margin-bottom: 16px;
    }

    .section-3 .detail-info-wrapper .detail-info-box  .subtitle{
      display: none;
    }

    .section-4 .header{
      color: black;
      font-size: 32px;
      font-weight: 800;
      line-height: 150%;
      font-family: 'Visby CF';
      margin-bottom: 16px;
    }

    .section-4 .subheader{
      color: black;
      filter: opacity(0.8);
      font-size: 16px;
      line-height: 175%;
      font-weight: 400;
    }

    .section-4 .doctor-wrapper{
      margin-top: 16px;
    }

    .section-4 .doctor-wrapper .doctor-box .doctor-avatar{
      max-width: 100%;
      height: auto;
    }

    .section-4 .doctor-wrapper .doctor-box .doctor-name{
      font-size: 20px;
    }

    .section-4 .doctor-wrapper .join-box .join-icon{
      max-width: 100%;
      height: auto;

    }

    .section-4 .doctor-wrapper .join-box .join-title{
      font-size: 20px;

    }





    
    .section-5{
      padding: 36px 0px;
    }

    .section-5 .title{
      color: white;
      font-size: 26px;
      margin-bottom: 8px;
    }

    .section-5 .subtitle{
      color: rgb(255, 255, 255, 80%);
      font-size: 16px;
      margin-bottom: 24px;
    }
    .section-5 .button-wrapper{
      justify-content: start !important;
    }

    .section-5 .button-wrapper .button{
      padding: 15px 20px;
      color: white;
      background-color: #010425;
      font-size: 16px;
      font-weight: 500;
      border-radius: 10px;
    }

    .section-5 .button-wrapper .button img{
      width: 24px;
    }



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
<script>
export default {}
</script>
