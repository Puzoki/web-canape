<template>
    <div class="services">
        <span class="services__title">наши услуги</span>
        <div v-for="service in services" class="services__card">
            <img :src="service.img" :alt="service.service_name">
            <div class="card__information">
                <div class="decoration top"></div>
                <span class="information__name">{{ service.service_name }}</span>
                <span class="information__price">{{ service.price }} ₽</span>
                <span class="information__period">в месяц</span>
                <div class="decoration bottom"></div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "services",
    data() {
        return {
            services: [
                {
                    img: 'confident-young-muscular-caucasian-athlete-practicing-gym-with-weights-male-model-doing-strength-exercises-training-his-upper-body-wellness-healthy-lifestyle-bodybuilding-concept.png',
                    service_name: 'тренажёрный зал',
                    price: 2500,
                },
                {
                    img: 'athlete-swimming-pool-full-shot.png',
                    service_name: 'бассейн',
                    price: 1200,
                },
                {
                    img: 'woman-doing-pilates-with-ball.png',
                    service_name: 'пилатес',
                    price: 1800,
                }
            ]
        }
    }
}
</script>

<style scoped>
.services {
    width: 1920px;
    height: 700px;
    padding: 205px 370px 95px 370px;
    box-sizing: border-box;

    position: absolute;
    left: 0px;
    top: 780px;

    display: flex;
    gap: 20px;

    background-color: #F4F4F4;
}

.services__title {
    position: absolute;
    width: 1180px;
    height: 45px;
    left: 370px;
    top: 100px;

    font-weight: bold;
    font-size: 35px;
    line-height: 45px;

    text-align: center;
    text-transform: uppercase;

    color: #000000;
}

.services__card {
    position: relative;
    width: 380px;
    height: 400px;
    cursor: pointer;
}

.services__card:hover .information__name {
    color: #95E82C;
}

img {
    width: 380px;
    height: 400px;
}

.card__information {
    position: absolute;
    display: flex;
    flex-direction: column;
}

.card__information span {
    position: absolute;
    left: 40px;
    width: 300px;
    height: 30px;
    line-height: 30px;

    text-align: center;
    color: #FFFFFF;
    text-transform: uppercase;
}

.information__name {
    top: -215px;
    font-weight: bold;
    font-size: 24px;
}

.information__price {
    top: -103px;
    font-weight: 400;
    font-size: 30px;
}

.information__period {
    top: -77px;
    font-weight: 400;
    font-size: 12px;
}

.decoration {
    background-color: #95E82C;
    position: absolute;
    left: 150px;
    transition: background-color 150ms;
}

.top {
    top: -406px;
    width: 80px;
    height: 6px;
}

.bottom {
    top: -18px;
    width: 80px;
    height: 12px;
}

@media (width <=768px) {}

@media (width <=340px) {}
</style>