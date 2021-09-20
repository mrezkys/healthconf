<template>
    <div class="dashboard">
        <div class="custom-nav">
            <div class="container-lg">
                <DashboardNavbar/>
            </div>
        </div>
        <div class="stacked-1">
            <div class="container-lg">
                <div class="stacked-content text-center">
                    <h4 class="header">Pilih layanan konsultasi {{$route.query.logintype}}</h4>
                </div> 
            </div>
        </div>
        <div class="section-1">
            <div class="container-lg">
                <div class="row menu-wrapper">

<!----------------- Guest Modal ------------------------->
                    <b-modal ref="guest-alert" class="guest-alert-modal" scrollable size="xl" title="Pemberitahuan" hide-footer >
                        <div class="content">
                            <p style="line-height: 150%">Kamu masuk sebagai tamu sehingga layanan berupa videocall tidak bisa kamu akses. Untuk mengaksesnya silahkan masuk dengan akun yang telah kamu buat sebelumnya, atau membuat akun baru.</p>
                        </div>
                    </b-modal>

<!----------------- covid VC ------------------------->
                    <b-modal id="modal-covid-vc" scrollable size="xl" hide-footer hide-header style="border-radius: 20px !important" >
                        <div class="konsultasi-form-modal">
                            <div class="header p-lg-0 p-2">
                                <div class="row d-flex justify-content-md-between p-lg-3">
                                    <h3 class="title">Formulir Konsultasi.</h3>
                                    <img class="company-logo" src="~assets/icons/logoblack.svg" alt="">
                                </div>
                            </div>
                            <div class="content">
                                <div class="col-lg-7 p-0 m-0">
                                    <p>Kamu memilih konsultasi tentang covid19 melalui video call. Sebelum itu, kamu harus mengisi formulir konfirmasi dibawah.</p>
                                </div>
                            </div>
                            <div class="form">
                                <div class="row">
                                    <div class="col-lg-6 form-wrapper">
                                        <select class="form-select" aria-label="Default select example">
                                            <option selected>Pilih Tanggal Konsultasi...</option>
                                            <option value="1">21 September 2021</option>
                                            <option value="2">22 September 2021</option>
                                            <option value="3">23 September 2021</option>
                                        </select>
                                    </div>
                                    <div class="col-lg-6 form-wrapper">
                                        <select class="form-select" aria-label="Default select example">
                                            <option selected>Pilih Jam Konsultasi...</option>
                                            <option value="1">08:00 - 10:00 WIB</option>
                                            <option value="2">10:00 - 12:00 WIB</option>
                                            <option value="3">13:00 - 15:00 WIB</option>
                                        </select>
                                    </div>
                                </div>
                            </div>
                            <div class="footer">                                    
                                <button class="btn btn-primary btn-lg daftar d-inline-block" @click="$bvModal.hide('modal-covid-vc')">Daftar Konsultasi</button>
                                <button type="button" class="btn btn-link d-inline-block my-auto ml-lg-2" @click="$bvModal.hide('modal-covid-vc')">Batal</button>
                            </div>
                        </div>
                    </b-modal>

<!----------------- mental VC ------------------------->
                    <b-modal id="modal-mental-vc" scrollable size="xl" hide-footer hide-header style="border-radius: 20px !important" >
                        <div class="konsultasi-form-modal">
                            <div class="header p-lg-0 p-2">
                                <div class="row d-flex justify-content-md-between p-lg-3">
                                    <h3 class="title">Formulir Konsultasi.</h3>
                                    <img class="company-logo" src="~assets/icons/logoblack.svg" alt="">
                                </div>
                            </div>
                            <div class="content">
                                <div class="col-lg-7 p-0 m-0">
                                    <p>Kamu memilih konsultasi tentang kesehatan mental melalui video call. Sebelum itu, kamu harus mengisi formulir konfirmasi dibawah.</p>
                                </div>
                            </div>
                            <div class="form">
                                <div class="row">
                                    <div class="col-lg-6 form-wrapper">
                                        <select class="form-select" aria-label="Default select example">
                                            <option selected>Pilih Tanggal Konsultasi...</option>
                                            <option value="1">21 September 2021</option>
                                            <option value="2">22 September 2021</option>
                                            <option value="3">23 September 2021</option>
                                        </select>
                                    </div>
                                    <div class="col-lg-6 form-wrapper">
                                        <select class="form-select" aria-label="Default select example">
                                            <option selected>Pilih Jam Konsultasi...</option>
                                            <option value="1">08:00 - 10:00 WIB</option>
                                            <option value="2">10:00 - 12:00 WIB</option>
                                            <option value="3">13:00 - 15:00 WIB</option>
                                        </select>
                                    </div>
                                </div>
                            </div>
                            <div class="footer">                                    
                                <button class="btn btn-primary btn-lg daftar d-inline-block" @click="$bvModal.hide('modal-mental-vc')">Daftar Konsultasi</button>
                                <button type="button" class="btn btn-link d-inline-block my-auto ml-lg-2" @click="$bvModal.hide('modal-mental-vc')">Batal</button>
                            </div>
                        </div>
                    </b-modal>

                    
<!----------------- covid chat ------------------------->
                    <b-modal id="modal-covid-chat" scrollable size="xl" hide-footer hide-header style="border-radius: 20px !important" >
                        <div class="konsultasi-form-modal">
                            <div class="header p-lg-0 p-2">
                                <div class="row d-flex justify-content-md-between p-lg-3">
                                    <h3 class="title">Formulir Konsultasi.</h3>
                                    <img class="company-logo" src="~assets/icons/logoblack.svg" alt="">
                                </div>
                            </div>
                            <div class="content">
                                <div class="col-lg-7 p-0 m-0">
                                    <p>Kamu memilih konsultasi tentang covid19 melalui chat. Sebelum itu, kamu harus mengisi formulir konfirmasi dibawah.</p>
                                </div>
                            </div>
                            <div class="form">
                                <div class="row">
                                    <div class="col-lg-6 form-wrapper">
                                        <select class="form-select" aria-label="Default select example">
                                            <option selected>Pilih Tanggal Konsultasi...</option>
                                            <option value="1">21 September 2021</option>
                                            <option value="2">22 September 2021</option>
                                            <option value="3">23 September 2021</option>
                                        </select>
                                    </div>
                                    <div class="col-lg-6 form-wrapper">
                                        <select class="form-select" aria-label="Default select example">
                                            <option selected>Pilih Jam Konsultasi...</option>
                                            <option value="1">08:00 - 10:00 WIB</option>
                                            <option value="2">10:00 - 12:00 WIB</option>
                                            <option value="3">13:00 - 15:00 WIB</option>
                                        </select>
                                    </div>
                                </div>
                            </div>
                            <div class="footer">                                    
                                <button class="btn btn-primary btn-lg daftar d-inline-block" @click="$bvModal.hide('modal-covid-chat')">Daftar Konsultasi</button>
                                <button type="button" class="btn btn-link d-inline-block my-auto ml-lg-2" @click="$bvModal.hide('modal-covid-chat')">Batal</button>
                            </div>
                        </div>
                    </b-modal>
                    
<!----------------- mental chat ------------------------->
                    <b-modal id="modal-mental-chat" scrollable size="xl" hide-footer hide-header style="border-radius: 20px !important" >
                        <div class="konsultasi-form-modal">
                            <div class="header p-lg-0 p-2">
                                <div class="row d-flex justify-content-md-between p-lg-3">
                                    <h3 class="title">Formulir Konsultasi.</h3>
                                    <img class="company-logo" src="~assets/icons/logoblack.svg" alt="">
                                </div>
                            </div>
                            <div class="content">
                                <div class="col-lg-7 p-0 m-0">
                                    <p>Kamu memilih konsultasi tentang kesehatan mental melalui chat. Sebelum itu, kamu harus mengisi formulir konfirmasi dibawah.</p>
                                </div>
                            </div>
                            <div class="form">
                                <div class="row">
                                    <div class="col-lg-6 form-wrapper">
                                        <select class="form-select" aria-label="Default select example">
                                            <option selected>Pilih Tanggal Konsultasi...</option>
                                            <option value="1">21 September 2021</option>
                                            <option value="2">22 September 2021</option>
                                            <option value="3">23 September 2021</option>
                                        </select>
                                    </div>
                                    <div class="col-lg-6 form-wrapper">
                                        <select class="form-select" aria-label="Default select example">
                                            <option selected>Pilih Jam Konsultasi...</option>
                                            <option value="1">08:00 - 10:00 WIB</option>
                                            <option value="2">10:00 - 12:00 WIB</option>
                                            <option value="3">13:00 - 15:00 WIB</option>
                                        </select>
                                    </div>
                                </div>
                            </div>
                            <div class="footer">                                    
                                <button class="btn btn-primary btn-lg daftar d-inline-block" @click="$bvModal.hide('modal-mental-chat')">Daftar Konsultasi</button>
                                <button type="button" class="btn btn-link d-inline-block my-auto ml-lg-2" @click="$bvModal.hide('modal-mental-chat')">Batal</button>
                            </div>
                        </div>
                    </b-modal>
                    
                    <div class="col-lg-3 col-md-6 p-2 menu-box" v-b-modal.modal-covid-vc>
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

                    <div class="col-lg-3 col-md-6 p-2 menu-box" v-b-modal.modal-mental-vc>
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
                    

                    <div class="col-lg-3 col-md-6 p-2 menu-box" v-b-modal.modal-mental-chat>
                        <div class="col-12 secondary">
                            <div class="tag-secondary">
                                <p>Chatting</p>
                            </div>
                            <img class="icon p-1" src="~assets/icons/chat.svg" alt="">
                            <h5 class="title">
                                Konsultasi Kesehatan Mental
                            </h5>
                        </div>
                    </div>
                    

                    <div class="col-lg-3 col-md-6 p-2 menu-box" v-b-modal.modal-covid-chat>
                        <div class="col-12 secondary">
                            <div class="tag-secondary">
                                <p>Chatting</p>
                            </div>
                            <img class="icon p-1" src="~assets/icons/chat.svg" alt="">
                            <h5 class="title">
                                Konsultasi Kesehatan Mental
                            </h5>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="section-2" id="sec2">
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
                    
                    <NuxtLink to="/dashboard/schedule-detail/22sep2021-0800WIB" style="text-decoration: none !important;">
                    <div class="schedule-box not-today d-flex justify-content-between">
                        <div class="col-md-8 col-lg-5 col-9">
                            <h5 class="title">Konsultasi tentang Kesehatan Mental dengan Dr. Jeremy Alam</h5>
                        </div>
                        <div class="datetime my-auto">
                            <p>Pagi</p>
                            <h5>08:00</h5>
                        </div>
                    </div>
                    </NuxtLink>
                    
                    <NuxtLink to="/dashboard/schedule-detail/22sep2021-1000WIB" style="text-decoration: none !important;">
                    <div class="schedule-box not-today d-flex justify-content-between">
                        <div class="col-md-8 col-lg-5 col-9">
                            <h5 class="title">Konsultasi tentang Covid 19 dengan Dr. Jessyca Mi</h5>
                        </div>
                        <div class="datetime my-auto">
                            <p>Pagi</p>
                            <h5>10:00</h5>
                        </div>
                    </div>
                    </NuxtLink>


                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    methods: {
        showGuestModal(){
            this.$refs['guest-alert'].show();
        },
        hideGuestModal(){
            this.$refs['guest-alert'].show();
        }
    },
    mounted(){
        if(this.$route.query.logintype == 'guest'){
            this.showGuestModal();
            console.log('berhasil');
        }
    }
}
</script>

<style scoped>


    .konsultasi-form-modal{
        padding: 30px 50px !important;
    }

    .konsultasi-form-modal .header .title{
        font-size: 34px;
        font-weight: 800;
        font-family: 'Visby CF';
    }

    .konsultasi-form-modal .content p{
        font-size: 18px;
        line-height: 175%;
    }

    .konsultasi-form-modal .form{
        margin-top: 32px;
    }

    .konsultasi-form-modal .form .form-select{
        width: 100%;
        padding: 15px 30px;
        border-radius: 10px;
    }

    .konsultasi-form-modal .footer{
        margin-top: 36px;
    }

    .konsultasi-form-modal .footer .btn{
        padding: 15px 30px;
    }

    .konsultasi-form-modal .form .daftar{
        padding: 15px 40px;
    }

    @media (max-width: 575.98px) {
       .konsultasi-form-modal{
           padding: 20px 16px !important;
       } 

        .konsultasi-form-modal .header .company-logo{
            display: none;
        }

        .konsultasi-form-modal .header .title{
            font-size: 26px;
        }

        .konsultasi-form-modal .content p{
            font-size: 14px;
            margin-bottom: 0px;
        }

        .konsultasi-form-modal .form .form-wrapper{
            margin-top: 16px;
        }

        .konsultasi-form-modal .footer .btn{
            font-size: 14px;
        }
    }

    @media (min-width: 575.98px) and (max-width: 1366px) {
        .konsultasi-form-modal .header .company-logo{
            display: none;
        }

        .konsultasi-form-modal .form .form-wrapper{
            margin-top: 24px;
        }
    }






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