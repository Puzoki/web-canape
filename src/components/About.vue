<template>
    <div class="about">
        <div class="about-flex-container">
            <div class="information">
                <span class="information__title">train hard</span>
                <span class="information__rating">фитнесс-клуб №1</span>
                <span class="information__words">С нами вы можете быть уверены в безопасности своего здоровья –
                    дипломированный тренерский состав всегда к вашим услугам. Наши клиенты весьма разноплановые люди:
                    профессиональные спортсмены, медийные персоны, менеджеры высшего и среднего звена, творческие личности и
                    домохозяйки – и к каждому из них у нас индивидуальный подход, соответствующий самым требовательным
                    запросам.</span>
            </div>
            <div class="statistics">
                <div class="year-of-foundation">
                    <p class="year-of-foundation__year">2005</p>
                    <p class="year-of-foundation__text">Год основания фитнесс-клуба</p>
                </div>
                <div class="number-of-coaches">
                    <p class="number-of-coaches__number">18</p>
                    <p class="number-of-coaches__coaches">Профессиональных тренеров</p>
                </div>
                <div class="number-of-clients">
                    <p class="number-of-clients__number">&#62;300</p>
                    <p class="number-of-clients__clients">Постоянных клиентов</p>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "about",
}
</script>

<style scoped>
.about {
    position: absolute;
    top: 1475px;

    width: 1920px;
    height: 546px;
    background-color: #FFFFFF;
}

.about-flex-container {
    position: absolute;
    top: 95px;
    left: 370px;

    display: flex;
    flex-direction: row;
    gap: 120px;

    width: 1180px;
    height: 446px;

    background-color: #FFFFFF;
}

.information {
    position: relative;
    width: 680px;
    height: 313px;
    display: flex;
    flex-direction: column;
    text-align: left;
}

.statistics {
    width: 380px;
    height: 339px;
    text-align: left;
}

.information__title {
    position: absolute;
    top: 0;

    width: 680px;
    height: 65px;

    font-weight: 700;
    font-size: 55px;
    line-height: 65px;

    color: black;
    text-transform: uppercase;
}

.information__rating {
    position: absolute;
    top: 82px;

    width: 680px;
    height: 45px;

    font-weight: 500;
    font-size: 24px;
    line-height: 45px;

    color: #95E82C;
    text-transform: uppercase;
}

.information__words {
    position: absolute;
    top: 157px;

    width: 680px;
    height: 156px;

    font-weight: 400;
    font-size: 18px;
    line-height: 26px;

    color: #444444;
}

.year-of-foundation {
    display: flex;
    flex-direction: row;
    gap: 23px;
}

.year-of-foundation__year {
    width: 129px;
    height: 65px;
    margin: 0 0 35px 0;

    font-weight: 400;
    font-size: 55px;
    line-height: 65px;
}

.year-of-foundation__text {
    width: 134px;
    height: 48px;
    margin: 9px 0 43px 0;

    font-weight: 500;
    font-size: 20px;
    line-height: 24px;
}

.number-of-coaches {
    height: 139px;

    display: flex;
    flex-direction: row;
    gap: 20px;

    border-top: solid 2px #95E82C;
    border-bottom: solid 2px #95E82C;
}

.number-of-coaches__number {
    width: 55px;
    height: 65px;
    margin: 35px 0 35px 0;

    font-weight: 400;
    font-size: 55px;
    line-height: 65px;
}

.number-of-coaches__coaches {
    width: 182px;
    height: 48px;
    margin: 44px 0 43px 0;

    font-weight: 500;
    font-size: 20px;
    line-height: 24px;
}

.number-of-clients {
    display: flex;
    flex-direction: row;
    gap: 20px;
}

.number-of-clients__number {
    width: 132px;
    height: 65px;
    margin: 35px 0 0 0;

    font-weight: 400;
    font-size: 55px;
    line-height: 65px;
}

.number-of-clients__clients {
    width: 116px;
    height: 48px;
    margin: 44px 0 0 0;

    font-weight: 500;
    font-size: 20px;
    line-height: 24px;
}

@media (width <=768px) {}

@media (width <=340px) {}
</style>