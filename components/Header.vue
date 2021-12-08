<template>
    <div>
        <b-navbar toggleable="lg" type="light" variant="light">
            <b-container>
                <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

                <b-collapse id="nav-collapse" is-nav>
                    <b-navbar-nav>
                        <b-nav-item href="#about" @click="gotoAbout()">
                            <span class="link">About</span>
                        </b-nav-item>
                        <b-nav-item href="#portfolio" @click="gotoPortfolio()">
                            <span class="link">Portfolio</span>
                        </b-nav-item>
                        <b-nav-item href="#socials" @click="gotoSocials()">
                            <span class="link">Social Media</span>
                        </b-nav-item>
                    </b-navbar-nav>
                </b-collapse>
            </b-container>
        </b-navbar>

        <header>
            <b-container>
                <b-row class="row">
                    <b-col cols="12" lg="6">
                        <div class="hero-text">
                            <h1>Hello!</h1>
                            <p>I'm a <span>Frontend</span> Web Developer</p>
                        </div>
                    </b-col>
                    <b-col cols="12" lg="6">
                        <div class="hero-image">
                            <img class="border-img" src="~/assets/hero-image-border.png" alt="border">
                            <img class="my-image" src="~/assets/hero-image.png" alt="my-image">
                        </div>
                    </b-col>
                </b-row>
            </b-container>
        </header>
    </div>
</template>

<script>
export default {
    methods: {
        gotoAbout() {
            this.$router.replace({ name: this.$route.name, hash: '#about' });          
        },
        gotoPortfolio() {
            this.$router.replace({ name: this.$route.name, hash: '#portfolio' });          
        },
        gotoSocials() {
            this.$router.replace({ name: this.$route.name, hash: '#socials' });          
        }
    }
}
</script>

<style scoped>

    .navbar {
        background-color: transparent !important;
        margin-top: 30px;
    }

    .navbar .navbar-toggler {
        -webkit-filter: invert(100%) sepia(28%) saturate(5743%) hue-rotate(311deg) brightness(92%) contrast(104%);
                filter: invert(100%) sepia(28%) saturate(5743%) hue-rotate(311deg) brightness(92%) contrast(104%);
        }

        .navbar .nav-link {
        position: relative;
        z-index: 2;
        display: -webkit-box;
        display: -ms-flexbox;
        display: flex;
        -webkit-box-pack: center;
            -ms-flex-pack: center;
                justify-content: center;
        -webkit-box-align: center;
            -ms-flex-align: center;
                align-items: center;
        margin-right: 40px;
    }

    .navbar .nav-link::before {
        content: "";
        width: 100%;
        height: 100%;
        position: absolute;
        top: 0;
        left: 0;
        background-color: #efb960;
        border-radius: 20px 5px;
        z-index: 1;
        -webkit-transition: -webkit-transform 0.6s;
        transition: -webkit-transform 0.6s;
        transition: transform 0.6s;
        transition: transform 0.6s, -webkit-transform 0.6s;
        -webkit-transform: scaleX(0);
                transform: scaleX(0);
        -webkit-transform-origin: 0 0;
                transform-origin: 0 0;
        -webkit-transition-timing-function: cubic-bezier(0.5, 1.6, 0.4, 0.7);
                transition-timing-function: cubic-bezier(0.5, 1.6, 0.4, 0.7);
    }

    .navbar .nav-link .link {
        font-size: 20px;
        color: #333 !important;
        font-weight: bold;
        position: relative;
        z-index: 2;
        -webkit-transition: 0.6s;
        transition: 0.6s;
        text-decoration: none;
    }

    .navbar .nav-link:hover::before {
        -webkit-transform: scaleX(1);
                transform: scaleX(1);
    }

    .navbar .nav-link:hover .link {
        color: #fff !important;
    }

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
        .navbar .navbar-nav {
            margin-top: 20px;
        }
        .navbar .navbar-nav .nav-link {
            padding-left: 15px;
            margin-bottom: 10px;
            width: 150px;
            -webkit-box-pack: start;
                -ms-flex-pack: start;
                    justify-content: start;
        }
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