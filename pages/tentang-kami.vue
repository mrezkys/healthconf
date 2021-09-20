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
                <p class="content">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Nunc aliquet bibendum enim facilisis gravida neque convallis a cras. Fusce id velit ut tortor pretium viverra suspendisse. Massa eget egestas purus viverra accumsan. Iaculis eu non diam phasellus vestibulum lorem sed. Pulvinar elementum integer enim neque volutpat ac tincidunt vitae.
                    <br> <br>
                     Nibh tellus molestie nunc non blandit massa enim. Arcu odio ut sem nulla pharetra. Mi tempus imperdiet nulla malesuada pellentesque elit. Massa eget egestas purus viverra accumsan in nisl. Vitae suscipit tellus mauris a diam maecenas. Nascetur ridiculus mus mauris vitae. Semper auctor neque vitae tempus quam pellentesque nec nam. Id eu nisl nunc mi ipsum faucibus vitae. Sed viverra ipsum nunc aliquet bibendum enim facilisis gravida. Augue eget arcu dictum varius duis at consectetur lorem donec.</p>
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