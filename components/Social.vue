<template>
    <b-container id="socials" class="social">
        <h2 class="text-center" data-aos="fade-up" data-aos-duration="500">You Can Find Me at</h2>
        <div class="social-media-row">
            <div class="social-link" data-aos="zoom-in" data-aos-duration="500">
                <a href="https://web.facebook.com/galih.p.33865?_rdc=1&_rdr" target="_blank">
                    <img src="~/assets/ic-facebook.svg" alt="social-icons">
                </a>
            </div>
            <div class="social-link" data-aos="zoom-in" data-aos-duration="500">
                <a href="https://www.instagram.com/_galihprihananto/" target="_blank">
                    <img src="~/assets/ic-instagram.svg" alt="social-icons">
                </a>
            </div>
            <div class="social-link" data-aos="zoom-in" data-aos-duration="500">
                <a href="https://www.linkedin.com/in/galih-prihananto/" target="_blank">
                    <img src="~/assets/ic-linkedin.svg" alt="social-icons">
                </a>
            </div>
            <div class="social-link" data-aos="zoom-in" data-aos-duration="500">
                <a href="https://dribbble.com/Galihpro_" target="_blank">
                    <img src="~/assets/ic-dribbble.svg" alt="social-icons">
                </a>
            </div>
        </div>
        <strong></strong>
    </b-container>
</template>

<style scoped>
    .social {
        padding-top: 80px;
        height: 100%;
    }

    .social h2 {
        font-size: 32px;
        font-weight: bold;
        line-height: 44px;
        color: #333;
        margin: 0;
    }

    .social .social-media-row {
        display: -webkit-box;
        display: -ms-flexbox;
        display: flex;
        -ms-flex-wrap: wrap;
            flex-wrap: wrap;
        -webkit-box-pack: justify;
            -ms-flex-pack: justify;
                justify-content: space-between;
        max-width: 600px;
        margin: 50px auto 0;
    }

    .social .social-media-row .social-link {
        width: 100px;
        height: 100px;
        background-color: #fff3e0;
        border-radius: 50%;
        display: -webkit-box;
        display: -ms-flexbox;
        display: flex;
        -webkit-box-pack: center;
            -ms-flex-pack: center;
                justify-content: center;
        -webkit-box-align: center;
            -ms-flex-align: center;
                align-items: center;
        -webkit-transition: 0.6s;
        transition: 0.6s;
    }

    .social .social-media-row .social-link img {
        -webkit-transition: 0.6s;
        transition: 0.6s;
        width: 100%;
    }

    .social .social-media-row .social-link:hover {
        background-color: #efb960;
    }

    .social .social-media-row .social-link:hover img {
        -webkit-filter: invert(97%) sepia(100%) saturate(0%) hue-rotate(69deg) brightness(104%) contrast(104%);
                filter: invert(97%) sepia(100%) saturate(0%) hue-rotate(69deg) brightness(104%) contrast(104%);
    }

    @media (min-width: 992px) {
        .social {
            padding-top: 160px;
        }
    }

    @media (max-width: 767px) {
        .social .social-media-row .social-link {
            width: 70px;
            height: 70px;
        }
        .social .social-media-row .social-link a {
            width: 70%;
        }
    }

    @media (max-width: 575px) {
        .social .social-media-row {
            -webkit-box-pack: center;
            -ms-flex-pack: center;
            justify-content: center;
        }
        .social .social-media-row .social-link {
            width: 40px;
            height: 40px;
            margin: 0 10px;
        }
        .social .social-media-row .social-link a {
            width: 20px;
        }
        .social .social-media-row .social-link a img {
            height: 20px;
        }
    }

    @media (max-width: 470px) {
        .social h2 {
            font-size: 26px;
            line-height: 32px;
        }
    }
</style>