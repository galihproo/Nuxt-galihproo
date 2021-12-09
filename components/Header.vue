<template>
    <div>
        <header>
            <b-container>
                <b-row class="row">
                    <b-col cols="12" lg="6">
                        <div class="hero-text" data-aos="fade-right" data-aos-duration="500">
                            <h1>Hello!</h1>
                            <p>I'm a <span>Frontend</span> Web Developer</p>
                        </div>
                    </b-col>
                    <b-col cols="12" lg="6">
                        <div class="hero-image" data-aos="zoom-in" data-aos-duration="1000">
                            <img class="border-img" src="~/assets/hero-image-border.png" alt="border">
                            <img class="my-image" src="~/assets/hero-image.png" alt="my-image">
                        </div>
                    </b-col>
                </b-row>
            </b-container>
        </header>
    </div>
</template>

<style scoped>

    header .hero-text {
        padding-top: 200px;
    }

    header .hero-text h1 {
        font-size: 60px;
        line-height: 62px;
        font-weight: bold;
        color: #333;
    }

    header .hero-text p {
        font-size: 28px;
        line-height: 30px;
        font-weight: 600;
        color: #333;
    }

    header .hero-text p span {
        color: #efb960;
        font-weight: bold;
    }

    header .hero-image {
        position: relative;
        -webkit-transition: 0.6s;
        transition: 0.6s;
        margin-right: 8%;
    }

    header .hero-image .border-img {
        width: 100%;
        height: 100%;
        position: absolute;
        top: 8%;
        left: 8%;
    }

    header .hero-image .my-image {
        width: 100%;
        z-index: 2;
        -webkit-transition: 0.6s;
        transition: 0.6s;
    }

    header .hero-image:hover .my-image {
        -webkit-transform: translate(8%, 8%);
                transform: translate(8%, 8%);
    }

    @media (min-width: 1200px) {
        header {
            height: calc(100vh - 62px);
        }
    }

    @media (max-width: 991px) {
        header {
            margin-top: 40px;
        }
        header .hero-text {
            padding-top: 0;
            margin-bottom: 40px;
        }
    }

    @media (max-width: 767px) {
        header {
            margin-top: 0;
        }
        header .hero-text {
            padding-top: 80px;
            margin-bottom: 80px;
            text-align: center;
        }
        header .hero-text h1 {
            margin-bottom: 14px;
        }
        header .hero-image {
            width: 70%;
            margin: 0 auto;
        }
    }

    @media (max-width: 575px) {
        header {
            height: auto;
        }
        header .hero-text {
            padding-top: 50px;
            margin-bottom: 50px;
        }
        header .hero-text p {
            font-size: 22px;
        }
        header .hero-image {
            width: 80%;
        }
    }

    @media (max-width: 400px) {
        header .hero-image {
            width: 90%;
        }
    }
</style>