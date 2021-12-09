<template>
    <b-navbar toggleable="lg" type="light" variant="light">
        <b-container>
            <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

            <b-collapse id="nav-collapse" is-nav>
                <b-navbar-nav>
                    <b-nav-item>
                        <NuxtLink to="/" class="link">Home</NuxtLink>
                    </b-nav-item>
                    <b-nav-item>
                        <NuxtLink to="/about" class="link">About</NuxtLink>
                    </b-nav-item>
                    <b-nav-item>
                        <NuxtLink to="/portfolio" class="link">Portfolio</NuxtLink>
                    </b-nav-item>
                    <b-nav-item>
                        <NuxtLink to="/socials" class="link">Social Media</NuxtLink>
                    </b-nav-item>
                </b-navbar-nav>
            </b-collapse>
        </b-container>
    </b-navbar>
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
    }
</style>