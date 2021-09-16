<template>
    <div class="dashboard">
        <div class="custom-nav">
            <div class="container-lg">
                <Navbar/>
            </div>
        </div>
        <div class="stacked-1">
            <div class="container-lg">
                <div class="stacked-content text-center">
                    <h4 class="header">Pilih layanan konsultasi</h4>
                </div> 
            </div>
        </div>
        <div class="section-1">
            <div class="container-lg">
                <div class="row menu-wrapper">
                    
                    <div class="col-lg-3 col-md-6 p-2 menu-box">
                        <div class="col-12 primary">
                            <div class="tag-primary">
                                <p>Video Call</p>
                            </div>
                            <img class="icon" src="~assets/icons/videocall.svg" alt="">
                            <h5 class="title">
                                Konsultasi Tentang Covid19
                            </h5>
                        </div>
                    </div>
                    

                    <div class="col-lg-3 col-md-6 p-2 menu-box">
                        <div class="col-12 primary">
                            <div class="tag-primary">
                                <p>Video Call</p>
                            </div>
                            <img class="icon" src="~assets/icons/videocall.svg" alt="">
                            <h5 class="title">
                                Konsultasi Kesehatan Mental
                            </h5>
                        </div>
                    </div>
                    

                    <div class="col-lg-3 col-md-6 p-2 menu-box">
                        <div class="col-12 secondary">
                            <div class="tag-secondary">
                                <p>Video Call</p>
                            </div>
                            <img class="icon" src="~assets/icons/videocall.svg" alt="">
                            <h5 class="title">
                                Konsultasi Kesehatan Mental
                            </h5>
                        </div>
                    </div>
                    

                    <div class="col-lg-3 col-md-6 p-2 menu-box">
                        <div class="col-12 secondary">
                            <div class="tag-secondary">
                                <p>Video Call</p>
                            </div>
                            <img class="icon" src="~assets/icons/videocall.svg" alt="">
                            <h5 class="title">
                                Konsultasi Kesehatan Mental
                            </h5>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="section-2">
            <div class="container-lg">
                <h3 class="header">Jadwal Konsultasi</h3>

                <div class="schedule-wrapper">
                    <p class="date ml-2">Konsultasi hari ini</p>

                    <NuxtLink to="/dashboard/schedule-detail/21sep2021-1300WIB" style="text-decoration: none !important;">
                    <div class="schedule-box today d-flex justify-content-between">
                        <div class="col-md-8 col-lg-5 col-9">
                            <h5 class="title">Konsultasi tentang Kesehatan Mental dengan Dr. Elissia S.Psi</h5>
                        </div>
                        <div class="datetime my-auto">
                            <p>Siang</p>
                            <h5>13:00</h5>
                        </div>
                    </div>
                    </NuxtLink>

                </div>

                <div class="schedule-wrapper">
                    <p class="date ml-2">22 September 2021</p>
                    
                    <div class="schedule-box not-today d-flex justify-content-between">
                        <div class="col-md-8 col-lg-5 col-9">
                            <h5 class="title">Konsultasi tentang Kesehatan Mental dengan Dr. Elissia S.Psi</h5>
                        </div>
                        <div class="datetime my-auto">
                            <p>Siang</p>
                            <h5>13:00</h5>
                        </div>
                    </div>

                    <div class="schedule-box not-today d-flex justify-content-between">
                        <div class="col-md-8 col-lg-5 col-9">
                            <h5 class="title">Konsultasi tentang Kesehatan Mental dengan Dr. Elissia S.Psi</h5>
                        </div>
                        <div class="datetime my-auto">
                            <p>Siang</p>
                            <h5>13:00</h5>
                        </div>
                    </div>


                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
    .dashboard .custom-nav{
        background-color: #010425;
    }
    .dashboard .stacked-1{
        background-color: #010425;
        min-height: 220px;
    }

    .dashboard .stacked-1 .stacked-content{
        color: white;
        padding-top: 40px;
    }

    .dashboard .stacked-1 .stacked-content .header{
        font-size: 22px;
        font-weight: 600;
    }

    .dashboard .section-1 .menu-wrapper{
        margin-top: -110px;
    }

    .dashboard .section-1 .menu-wrapper .menu-box{
        cursor: pointer;
    }

    .dashboard .section-1 .menu-wrapper .menu-box .primary{
        background-color: #07133A;
        border-radius: 20px;
        color: white;
        padding: 30px 30px;
    }

    .dashboard .section-1 .menu-wrapper .menu-box .secondary{
        background-color: #9FD0F9;
        border-radius: 20px;
        color: black;
        padding: 30px 30px;
    }


    .dashboard .section-1 .menu-wrapper .menu-box .icon{
        width: 44px;
        margin-left: 20px;
    }
    .dashboard .section-1 .menu-wrapper .menu-box .title{
        line-height: 150%;
        font-weight: 800;
        margin-top: 14px;
        font-family: 'Visby CF';
        font-size: 24px;
    }

    .dashboard .section-1 .menu-wrapper .menu-box .tag-primary{
        padding: 8px 20px;
        background-color: rgb(255, 255, 255, 10%);
        color: white;
        border-radius: 10px;
        display: inline-block;

    }

    .dashboard .section-1 .menu-wrapper .menu-box .tag-primary p{
        padding: 0px;
        margin: 0px;
        font-weight: 500;
    }

    .dashboard .section-1 .menu-wrapper .menu-box .tag-secondary{
        padding: 8px 20px;
        background-color: #87C4F7;
        color: black;
        border-radius: 10px;
        display: inline-block;

    }

    .dashboard .section-1 .menu-wrapper .menu-box .tag-secondary p{
        padding: 0px;
        margin: 0px;
        font-weight: 500;
    }

    .dashboard .section-2{
        margin-top: 40px;
        padding-top: 20px;
        padding-bottom: 80px;
    }

    .dashboard .section-2 .header{
        font-size: 32px;
        font-family: 'Visby CF';
        font-weight: 800;
    }

    .dashboard .section-2 .schedule-wrapper{
        margin-top: 30px;
    }

    .dashboard .section-2 .schedule-wrapper .date{
        font-size: 18px;
        color: grey;
    }

    .dashboard .section-2 .schedule-wrapper .today{
        color: white;
        background-color: #108AEE;
    }

    .dashboard .section-2 .schedule-wrapper .not-today{
        color: black;
        background-color: white;
        border: 1px solid #9FD0F9;
    }

    .dashboard .section-2 .schedule-wrapper .schedule-box{
        padding: 30px 40px;
        border-radius: 20px;
        margin-top: 20px;
        cursor: pointer;
    }   
    
    .dashboard .section-2 .schedule-wrapper .schedule-box .title{
        line-height: 175%;
        font-weight: 600;
        font-size: 20px;
        margin: 0;
    }

    .dashboard .section-2 .schedule-wrapper .schedule-box .datetime p{
        margin-bottom: 8px;
    }

    .dashboard .section-2 .schedule-wrapper .schedule-box .datetime h5{
        font-weight: 800;
        font-size: 20px;
        font-family: 'Visby CF';
    }

    /* Mobile Responsive */

    
    @media (max-width: 575.98px) {
        .dashboard .stacked-1{
            background-color: #010425;
            min-height: 180px;
        }

        .dashboard .stacked-1 .stacked-content .header{
            font-size: 18px;
            font-weight: 600;
        }

        .dashboard .section-1 .menu-wrapper{
            margin-top: -100px;
        }

        .dashboard .section-1 .menu-wrapper .menu-box .primary{
            background-color: #07133A;
            border-radius: 20px;
            color: white;
            padding: 20px;
        }

        .dashboard .section-1 .menu-wrapper .menu-box .secondary{
            background-color: #9FD0F9;
            border-radius: 20px;
            color: black;
            padding: 20px;
        }

        .dashboard .section-1 .menu-wrapper .menu-box .icon{
            width: 28px;
            margin-left: 20px;
        }
        .dashboard .section-1 .menu-wrapper .menu-box .title{
            line-height: 150%;
            font-weight: 800;
            margin-top: 14px;
            font-family: 'Visby CF';
            font-size: 20px;
        }

        .dashboard .section-1 .menu-wrapper .menu-box .tag-primary{
            padding: 8px 20px;
            background-color: rgb(255, 255, 255, 10%);
            color: white;
            border-radius: 10px;
            display: inline-block;

        }

        .dashboard .section-1 .menu-wrapper .menu-box .tag-primary p{
            font-size: 14px;
            padding: 0px;
            margin: 0px;
            font-weight: 500;
        }

        .dashboard .section-1 .menu-wrapper .menu-box .tag-secondary p{
            font-size: 14px;

        }

        .dashboard .section-2{
            margin-top: 16px;
        }

        .dashboard .section-2 .header{
            font-size: 20px;
            text-align: center;
        }

        .dashboard .section-2 .schedule-wrapper{
            margin-top: 20px;
        }

        .dashboard .section-2 .schedule-wrapper .date{
            text-align: center;
            font-size: 14px;
        }

        .dashboard .section-2 .schedule-wrapper .schedule-box{
            padding: 20px;
            border-radius: 20px;
            margin-top: 16px;
            cursor: pointer;
        }   

        .dashboard .section-2 .schedule-wrapper .schedule-box .title{
            font-size: 16px;
            line-height: 150%;
        }

        .dashboard .section-2 .schedule-wrapper .schedule-box .datetime p{
            margin-bottom: 8px;
            font-size: 14px;
        }

        .dashboard .section-2 .schedule-wrapper .schedule-box .datetime h5{
            font-weight: 800;
            font-size: 16px;
            font-family: 'Visby CF';
        }
    }

</style>