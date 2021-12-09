<template>
    <b-container class="skills">
        <h2 class="text-center" data-aos="fade-up" data-aos-duration="500">My Skills</h2>
        <div class="skills-row">
            <div class="skill-item" data-aos="fade-up" data-aos-duration="500" data-aos-delay="0">
                <img class="icon-skill" src="~/assets/ic-html5.svg" alt="icon-skill">
                <img class="ic-border" src="~/assets/ic-html5-border.svg" alt="icon-skill">
            </div>
            <div class="skill-item" data-aos="fade-up" data-aos-duration="500" data-aos-delay="500">
                <img class="icon-skill" src="~/assets/ic-css3.svg" alt="icon-skill">
                <img class="ic-border" src="~/assets/ic-css3-border.svg" alt="icon-skill">
            </div>
            <div class="skill-item" data-aos="fade-up" data-aos-duration="500" data-aos-delay="1000">
                <img class="icon-skill" src="~/assets/ic-js.svg" alt="icon-skill">
                <img class="ic-border" src="~/assets/ic-js-border.svg" alt="icon-skill">
            </div>
            <div class="skill-item" data-aos="fade-up" data-aos-duration="500" data-aos-delay="1500">
                <img class="icon-skill" src="~/assets/ic-bootstrap.svg" alt="icon-skill">
                <img class="ic-border" src="~/assets/ic-bootstrap-border.svg" alt="icon-skill">
            </div>
            <div class="skill-item" data-aos="fade-up" data-aos-duration="500" data-aos-delay="2000">
                <img class="icon-skill" src="~/assets/ic-react.svg" alt="icon-skill">
                <img class="ic-border" src="~/assets/ic-react-border.svg" alt="icon-skill">
            </div>
            <div class="skill-item" data-aos="fade-up" data-aos-duration="500" data-aos-delay="2500">
                <img class="icon-skill" src="~/assets/ic-webflow.svg" alt="icon-skill">
                <img class="ic-border" src="~/assets/ic-webflow-border.svg" alt="icon-skill">
            </div>
        </div>
    </b-container>
</template>

<style scoped>
    .skills h2 {
        font-size: 32px;
        font-weight: bold;
        line-height: 44px;
        color: #333;
        margin: 0;
    }

    .skills .skills-row {
        display: -webkit-box;
        display: -ms-flexbox;
        display: flex;
        -webkit-box-pack: justify;
            -ms-flex-pack: justify;
                justify-content: space-between;
        max-width: 720px;
        -ms-flex-wrap: wrap;
            flex-wrap: wrap;
        margin: 30px auto 0;
    }

    .skills .skills-row .skill-item {
        width: 80px;
        height: 80px;
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
        position: relative;
    }

    .skills .skills-row .skill-item .icon-skill {
        width: 100%;
        height: 100%;
        -webkit-transition: .4s;
        transition: .4s;
    }

    .skills .skills-row .skill-item .ic-border {
        position: absolute;
        top: 10%;
        left: 10%;
        width: 100%;
        height: 100%;
    }

    .skills .skills-row .skill-item:hover .icon-skill {
        -webkit-transform: translate(10%, 10%);
                transform: translate(10%, 10%);
    }

    @media (max-width: 1199px) {
        .skills {
            margin-top: 120px;
        }
    }

    @media (max-width: 767px) {
        .skills {
            margin-top: 300px;
        }
    }

    @media (max-width: 575px) {
        .skills {
            margin-top: 100px;
        }
        .skills .skills-row {
            padding: 0 40px;
        }
        .skills .skills-row .skill-item {
            width: 50px;
            height: 50px;
        }
    }

    @media (max-width: 470px) {
        .skills h2 {
            font-size: 26px;
            line-height: 32px;
        }
    }

    @media (max-width: 400px) {
        .skills .skills-row {
            padding: 0 20px;
            -ms-flex-wrap: wrap;
            flex-wrap: wrap;
            justify-content: center;
        }
        .skills .skills-row .skill-item {
            margin: 15px 10px;
        }
    }
</style>