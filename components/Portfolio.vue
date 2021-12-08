<template>
    <b-container id="portfolio" class="portfolio">
        <h2 class="text-center">My Recent Portfolio</h2>
        <div class="row portfolio-row">
            <b-col cols="12" sm="6" lg="4" class="card-portfolio">
                <a href="https://semarvest.vercel.app/" target="_blank">
                    <div class="portfolio-content">
                        <img src="~/assets/portfolio3-img.png" alt="portfolio-image">
                    </div>
                </a>
            </b-col>
            <b-col cols="12" sm="6" lg="4" class="card-portfolio">
                <a href="https://galihproo.github.io/CourseIn-Online-Course-Website/" target="_blank">
                    <div class="portfolio-content">
                        <img src="~/assets/portfolio2-img.png" alt="portfolio-image">
                    </div>
                </a>
            </b-col>
            <b-col cols="12" sm="6" lg="4" class="card-portfolio">
                <a href="https://galihproo.github.io/TravellinKuy-Website/" target="_blank">
                    <div class="portfolio-content">
                        <img src="~/assets/portfolio-img.png" alt="portfolio-image">
                    </div>
                </a>
            </b-col>
        </div>
    </b-container>
</template>

<style scoped>
    .portfolio {
        margin-top: 100px;
    }

    .portfolio h2 {
        font-size: 32px;
        font-weight: bold;
        line-height: 44px;
        color: #333;
        margin: 0;
    }

    .portfolio .portfolio-row .portfolio-content {
        background-color: #fff3e0;
        width: 300px;
        height: 300px;
        border-radius: 100px 20px;
        margin: 40px 0 0;
        -webkit-box-shadow: 8px 8px 40px #e4e4e4;
                box-shadow: 8px 8px 40px #e4e4e4;
    }

    .portfolio .portfolio-row .portfolio-content img {
        width: 100%;
        height: 100%;
        border-radius: 100px 20px;
        object-fit: cover;
    }

    @media (max-width: 991px) {
        .portfolio .portfolio-row {
            -webkit-box-pack: center;
            -ms-flex-pack: center;
            justify-content: center;
        }
    }

    @media (max-width: 767px) {
        .portfolio .portfolio-row .portfolio-content {
            width: 100%;
        }
    }

    @media (max-width: 575px) {
        .portfolio .portfolio-row {
            display: block;
        }
        .portfolio .portfolio-row .card-portfolio {
            max-width: 60%;
            margin: 10px auto;
        }
    }

    @media (max-width: 470px) {
        .portfolio h2 {
            font-size: 26px;
            line-height: 32px;
        }
        .portfolio .portfolio-row .card-portfolio {
            max-width: 100%;
        }
    }
</style>