<template>
    <section class="competencies">
        <div class="container">
            <h2 class="competencies__title">Ключевые компетенции</h2>
            <div class="competencies__blocks">
                <div class="competencies__block">
                    <h3 class="competencies__block-title">Front-end разработка</h3>
                    <div class="competencies__block-images">
                        <img class="competencies__block-img" src="@/assets/img/react-logo.svg" alt="react logo">
                        <img class="competencies__block-img" src="@/assets/img/vue-logo.svg" alt="vue logo">
                    </div>
                    <p class="competencies__block-technology">ReactJS, VueJS</p>
                    <p class="competencies__block-description">
                        HTML5, CSS3, Stylus, SCSS/SASS, LESS, PostCSS, JS (ES5, ES6, ESNext), Webpack, Gulp, Yarn, Jade, Nuxt, Quasar Framework, Vuetify, Ant Framework,
                    </p>
                </div>
                <div class="competencies__block">
                    <h3 class="competencies__block-title">Back-end разработка</h3>
                    <div class="competencies__block-images">
                        <img class="competencies__block-img" src="@/assets/img/python-logo.svg" alt="react logo">
                        <img class="competencies__block-img" src="@/assets/img/django-logo.svg" alt="vue logo">
                    </div>
                    <p class="competencies__block-technology">Python, Django</p>
                    <p class="competencies__block-description">
                        Django REST API, Scrapy & Beautifulsoup, Docker, CI/CD, Kubernetes, PostgreSQL, MongoDB, Celery, RabbitMQ, Jinja2, Ansible, AWS
                    </p>
                </div>
                <div class="competencies__block">
                    <h3 class="competencies__block-title">Q/A тестирование</h3>
                    <div class="competencies__block-images">
                        <img class="competencies__block-img" src="@/assets/img/selenium-logo.svg" alt="react logo">
                        <img class="competencies__block-img" src="@/assets/img/zabbix-logo.svg" alt="vue logo">
                    </div>
                    <p class="competencies__block-technology">Selenium, Zabbix</p>
                    <p class="competencies__block-description">
                        Функциональное тестирование, нагрузочное, кроссбраузерное и регрессионное
                    </p>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss">
.competencies {
    padding-bottom: 140px;
    &__title {
        font-weight: 800;
        font-size: 48px;
        line-height: 59px;
        text-align: center;
        padding-bottom: 86px;
    }
    &__blocks {
        display: grid;
        grid-template: 1fr / repeat(3, 1fr);
        gap: 53px;
    }
    &__block {
        display: grid;
        grid-template: 74px 48px 50px 1fr / 1fr;
        &-title {
            font-weight: 800;
            font-size: 24px;
            line-height: 29px;
            padding-bottom: 52px;
        }
        &-images {
            display: flex;
            align-items: center;
        }
        &-img {
            margin-right: 25px;
        }
        &-technology {
            font-weight: 500;
            font-size: 18px;
            line-height: 22px;
            padding-top: 28px;
        }
        &-description {
            color: $text-color-blur;
            line-height: 24px;
            padding-top: 16px;
        }
    }
}
</style>