<template>
    <div class="schedule-detail">
        <div class="custom-nav ">          
            <div class="container-lg">
                <Navbar/>
            </div>
        </div>
        <div class="section-1">
            <div class="container-lg">
                <div class="row d-flex justify-content-between">                                 
                    <div class="schedule-info col-lg-6 col-md-8">
                        <h5 class="date">13:00 WIB | 21 September 2021</h5>
                        <h2 class="title">Konsultasi Kesehatan Mental dengan Dr. Elissia S.Psi</h2>
                        <button class="btn btn-primary">Konsultasi Sekarang</button>
                    </div>
                    <div class="col-md-3 doctor-image">
                        <img src="~assets/images/elisprofile.png" class="img-fluid" alt="">
                    </div>
                </div>
            </div>
        </div>
        <div class="section-2">
            <div class="container-lg">
                <div class="file-wrapper p-2">
                    <p class="header ml-2">Berkas konsultasi</p>

                    <div class="row file-box d-flex justify-content-md-between">
                        <div class="col-md-8 col-lg-5 col-12">
                            <h5 class="title">Rekaman Konsultasi</h5>
                        </div>
                        <div class="status my-auto col-sm-12 col-md-4 text-md-right">
                            <p>Belum Tersedia</p>
                        </div>
                    </div>
                    <div class="row file-box d-flex justify-content-md-between">
                        <div class="col-md-8 col-lg-5 col-12">
                            <h5 class="title">Asesment Diri</h5>
                        </div>
                        <div class="status my-auto col-sm-12 col-md-4 text-md-right">
                            <p>namapasien.pdf</p>
                        </div>
                    </div>

                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
    .schedule-detail .custom-nav{
        background-color: #010425;
    }

    .schedule-detail .section-1{
        background-color: #010425;
        padding-top: 50px;
        padding-bottom: 50px;
        color: white;
        background-image: url(~assets/images/background-accent.png);
        background-size: cover;
        background-position: bottom;
    }

    .schedule-detail .section-1 .schedule-info .date{
        font-size: 18px;
        margin-bottom: 18px;
    }

    .schedule-detail .section-1 .schedule-info .title{
        line-height: 150%;
        font-weight: 800;
        font-family: 'Visby CF';
        margin-bottom: 40px;
    }

    .schedule-detail .section-1 .schedule-info .btn{
        font-size: 20px;
        font-weight: 500;
        padding: 20px 30px;
    }

    .schedule-detail .section-2{
        padding-top: 40px;
        padding-bottom: 80px;
    }

    .schedule-detail .section-2 .file-wrapper .header{
        font-size: 18px;
        color: grey;
    }


    .schedule-detail .section-2 .file-wrapper .file-box{
        padding: 30px 40px;
        border-radius: 20px;
        margin-top: 24px;
        cursor: pointer;
        color: black;
        background-color: white;
        border: 1px solid #9FD0F9;
    }

    .schedule-detail .section-2 .file-wrapper .file-box .title{
        line-height: 175%;
        font-weight: 600;
        font-size: 20px;
        margin: 0;
    }

    .schedule-detail .section-2 .file-wrapper .file-box .status p{
        margin: 0;
        font-weight: 500;
        color: grey;
    }



    /* Mobile Responsive */

    
    @media (max-width: 575.98px) {

        .schedule-detail .section-1{
            padding-top: 30px;
            padding-bottom: 50px;
        }
        .schedule-detail .section-1 .schedule-info .date{
            font-size: 14px;
            margin-bottom: 18px;
        }

        .schedule-detail .section-1 .schedule-info .title{
            line-height: 150%;
            font-size: 24px;
            font-weight: 800;
            font-family: 'Visby CF';
            margin-bottom: 24px;
        }

        .schedule-detail .section-1 .schedule-info .btn{
            font-size: 16px;
            font-weight: 500;
            padding: 16px 24px;
        }


        .schedule-detail .section-1 .doctor-image{
            display: none;
        }

        .schedule-detail .section-2 .file-wrapper .file-box{
            padding: 20px 16px ;
        }


    }
</style>