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
                        <h1 class="header">Tentang Kami</h1>
                        <p class="subheader"><strong>Healthconf</strong> adalah inisiatif para dokter yang menjadi relawan untuk memberi kontribusi ditengah pandemi melalui pemberian konsultasi gratis.</p>
                    </div>
                    <div class="col-md-6 offset-md-1">
                        <img src="~assets/images/doctor-group.jpg" alt="" class="img-fluid">
                    </div>
                </div>
            </div>
        </div>
        <div class="section-2">
            <div class="container-lg">
                <h4 class="header">Berawal Dari...</h4>
                <p class="content">Berawal dari inisiatif para relawan yang pada awalnya berjumlah 3 orang. Healthconf dibangun didasari oleh keinginan untuk membantu sesama oleh ketiga dokter tersebut. Fokus utamanya adalah pemberian konsultasi terhadap masyarakat yang membutuhkan bimbingan, saran, dan penenang di situasi pandemi yang melanda sekarang.                
                    <br> <br>
                Hadirnya pandemi covid 19 ditengah masyarakat membuat situasi menjadi sangat memprihatinkan. Selain dampak dari pandemi ini sendiri yaitu penyebaran dan infeksi virus corona, pandemi ini juga berdampak pada mental masyarakat. Ditambah dengan pembatasan mobilisasi dan anjuran untuk diam dirumah saja memperparah kondisi mental masyarakat karena kurangnya interaksi dengan orang lain dan juga sulitnya akses untuk ke rumah sakit langsung. 
                    <br> <br>

                Healthconf hadir untuk mengatasi masalah tersebut. Dengan mengedepankan fitur konsultasi online berbasis chat dan video call, kami berharap bisa membantu banyak masyarakat. Dimulai dari 3 dokter pendiri, kini Healthconf telah memiliki lebih dari 20 Relawan yang siap membantu. Kami juga membuka kesempatan bagi para proffesional yang hendak menjadi relawan. Kedepannya, healthconf akan hadir dengan inovasi inovasi baru yang masih dalam proses pengembangan.
                </p>
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
        background-color: #07133A;
        padding-top: 46px;
        padding-bottom: 72px;
        color: white;
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

    .section-1 img{
        border-radius: 20px;
    }

    .section-2{
        padding: 52px 0;
    }

    .section-2 .header{
        font-size: 32px;
        font-weight: 800;
        font-family: 'Visby CF';
        margin-bottom: 32px;
    }

    .section-2 .content{
        font-size: 18px;
        line-height: 175%;
    }

    @media (max-width: 1024px) {
        .section-1{
            padding-top: 26px;
        }
        .section-1 .header{
            font-size: 32px;
            margin-bottom: 16px;
        }

        .section-1 .subheader{
            font-size: 16px;
            margin-bottom: 32px;
        }

        .section-2{
            padding: 32px 0;
        }

        .section-2 .header{
            font-size: 32px;
            margin-bottom: 16px;
        }

        .section-2 .content{
            font-size: 16px;
        }
    }
</style>