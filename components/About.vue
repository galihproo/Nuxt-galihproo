<template>
    <b-container id="about" class="about">
        <h2 class="text-center" data-aos="fade-up" data-aos-duration="500">About Me</h2>
        <div class="row">
            <div class="col-12 col-lg-6">
                <div class="about-card" data-aos="fade-right" data-aos-duration="1000">
                    <div class="title">Profile</div>
                    <table class="content">
                        <tr>
                            <td>Full Name</td>
                            <td>Galih Prihananto</td>
                        </tr>
                        <tr>
                            <td>Date of Birth</td>
                            <td>1 June 2003</td>
                        </tr>
                        <tr>
                            <td>Email</td>
                            <td>
                                <a href="mailto:galihprihananto29@gmail.com?">galihprihananto29@gmail.com</a>
                            </td>
                        </tr>
                        <tr>
                            <td>Address</td>
                            <td>Purwokerto, Central Java, Indonesia</td>
                        </tr>
                    </table>
                </div>
            </div>
            <div class="col-12 col-lg-6">
                <div class="about-card" data-aos="fade-left" data-aos-duration="1000">
                    <div class="title">Education</div>
                    <table class="content">
                        <tr>
                            <td>SDN 2 Karang Pucung</td>
                            <td>2009 - 2015</td>
                        </tr>
                        <tr>
                            <td>SMP Negeri 8 Purwokerto</td>
                            <td>2015 - 2018</td>
                        </tr>
                        <tr>
                            <td>SMK Telkom Purwokerto</td>
                            <td>2018 - 2021</td>
                        </tr>
                    </table>
                </div>
            </div>
        </div>
    </b-container>
</template>

<style scoped>

    .about {
        padding-top: 80px;
    }

    .about h2 {
        font-size: 32px;
        font-weight: bold;
        line-height: 44px;
        color: #333;
        margin: 0;
    }

    .about .about-card {
        background-color: #fff3e0;
        width: 100%;
        min-height: 360px;
        color: #333;
        border-radius: 50px;
        padding: 40px;
        margin-top: 50px;
    }

    .about .about-card .title {
        background-color: #efb960;
        width: 160px;
        padding: 10px;
        display: -webkit-box;
        display: -ms-flexbox;
        display: flex;
        -webkit-box-pack: center;
            -ms-flex-pack: center;
                justify-content: center;
        -webkit-box-align: center;
            -ms-flex-align: center;
                align-items: center;
        font-size: 24px;
        color: #fff3e0;
        font-weight: 600;
        border-radius: 20px;
        }

    .about .about-card .content {
        border: none;
        width: 100%;
        margin-top: 40px;
    }

    .about .about-card .content tr td,
    .about .about-card .content tr a {
        color: #333;
        font-size: 18px;
    }

    .about .about-card .content tr td {
        padding: 15px 0;
    }

    @media (min-width: 992px) {
        .about {
            height: 100vh;
        }
    }

    @media (max-width: 575px) {
        .about h2 {
            font-size: 32px;
            font-weight: bold;
            line-height: 44px;
            color: #333;
            margin: 0;
        }
        .about .about-card {
            min-height: 320px;
        }
        .about .about-card .title {
            font-size: 18px;
            width: 140px;
            border-radius: 16px;
        }
        .about .about-card tr {
            margin-bottom: 16px;
        }
        .about .about-card tr td,
        .about .about-card tr a {
            color: #333;
            font-size: 15px;
        }
    }

    @media (max-width: 470px) {
        .about h2 {
            font-size: 26px;
            line-height: 32px;
        }
        .about .about-card {
            padding: 20px;
        }
        .about .about-card .title {
            font-size: 16px;
            width: 120px;
            border-radius: 17px;
            margin: 0 auto;
        }
        .about .about-card .content tr td,
        .about .about-card .content tr a {
            color: #333;
            font-size: 15px;
            margin-bottom: 16px;
        }
    }

    @media (max-width: 340px) {
        .about .about-card .content tr td,
        .about .about-card .content tr a {
            color: #333;
            font-size: 13px;
            margin-bottom: 16px;
        }
    }
</style>