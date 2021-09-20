<template>
    <div>
        <div class="navbar-wrapper">
            <div class="container-lg">
                <Navbar/> 
            </div>
        </div>
        <div class="section-1">
            <div class="container-lg">
                <div class="row">
                    <div class="col-md-5 my-auto">
                        <h1 class="header">Program Kami</h1>
                        <p class="subheader">Kamu bisa menkonsultasikan tentang kesehatan di masa pandemi seperti tentang Covid19 atau tentang Kesehatan Mental secara virtual dengan layanan chat atau video call.</p>
                    </div>
                    <div class="col-md-6 pl-md-5 offset-md-1 image-wrapper">
                        <img src="~assets/images/elis.png" alt="" class="img-fluid">
                    </div>
                </div>
            </div>
        </div>
    <div class="section-2">
      <div class="container-lg">
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
                  <h3 class="title">Konsultasi Covid & Mental melalui Video Call</h3>
                  <p class="subtitle">Konsultasi seputar covid dan mental health secara gratis.</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
        <div class="section-3">
          <div class="container-lg">            
            <div class="row">
              <div class="col-md-6 photo-wrapper-1">
              </div>
              <div class="col-md-6 photo-wrapper-2">
              </div>
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
        background-image: url(~assets/images/background-accent.png);
        background-size: cover;
        background-position: bottom;
        background-repeat: no-repeat;
        color: white;
        padding-bottom: 40px;
        background-color: #07133A;
    }

    .section-1 .header{
        font-size: 50px;
        font-weight: 800;
        font-family: 'Visby CF';
        line-height: 150%;
        margin-bottom: 36px;
    }

    .section-1 .subheader{
        font-size: 20px;
        line-height: 175%;
    }


    .section-2{
        padding: 56px 0px;
        background-color: #010425;

    }

    .section-2 .detail-info-wrapper .icon-box{
        width: 180px;
        height: 180px;
        border-radius: 20px;
        background-color: #07133A;
    }

    .section-2 .detail-info-wrapper .detail-info-box{
        padding-left: 32px;
    }

    .section-2 .detail-info-wrapper .detail-info-box  .title{
        font-size: 26px;
        font-family: 'Visby CF';
        font-weight: 800;
        line-height: 150%;
        margin-bottom: 16px;
        color: white;
    }

    .section-2 .detail-info-wrapper .detail-info-box  .subtitle{
        font-size: 16px;
        color: white;
        line-height: 175%;
        margin: 0;
    }

    .section-3 {
      padding: 40px 0px;
        background-color: #010425;
    }

    .section-3 .photo-wrapper-1{
      min-height: 500px;
      background-image: url('~assets/images/1.jpg');
      background-size: cover;
      border-radius: 20px 0 0 0;
    }

    .section-3 .photo-wrapper-2{
      min-height: 500px;
      background-image: url('~assets/images/2.jpg');
      background-size: cover;
      border-radius: 0 20px 0 0;
    }

    @media (max-width: 1024px){
      .section-1{
        padding-top: 16px;
      }
      .section-1 .header{
        font-size: 32px;
        margin-bottom: 16px;
      }

      .section-1 .subheader{
        font-size: 16px;
        margin-bottom: 8px;
      }

      .section-1 .image-wrapper{
        padding-right: 56px;
      }

      .section-2 .info-box .title{
        color: black;
        font-size: 32px;
        margin-bottom: 16px;
        margin-top: 32px;
      }

      .section-2 .detail-info-wrapper{
        margin-top: 24px;
      }

      .section-2 .detail-info-wrapper .icon-box{
        width: 80px;
        height:80px;
        padding: 24px;
        border-radius: 20px;
        background-color: #07133A;
      }

      .section-2 .info{
        margin-top: 8px;
      }
      .section-2 .detail-info-wrapper .icon-box img{
        width: 48px;
      }

      .section-2 .detail-info-wrapper .detail-info-box{
        padding-left: 16px;
      }

      .section-2 .detail-info-wrapper .detail-info-box  .title{
        font-size: 19px;
        font-family: 'Visby CF';
        font-weight: 700;
        line-height: 150%;
        margin-bottom: 16px;
      }

      .section-3 .detail-info-wrapper .detail-info-box  .subtitle{
        display: none;
      }

      .section-3{
        display: none;
      }



    }
</style>