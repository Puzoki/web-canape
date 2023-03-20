<template>
    <div class="top">
        <img class="logo" src="/logo.svg" alt="logo">
        <div class="entry">
            <p><span>инвестируйте</span> в своё здоровье</p>
            <span>Ждем вас в нашем фитнес-клубе</span>
            <button>записаться</button>
        </div>
    </div>
    <navigation></navigation>
</template>

<script>
import navigation from './Navigation.vue'

export default {
    name: "top",
    components: {
        navigation,
    },
}
</script>

<style scoped>
.top {
    width: 1920px;
    height: 780px;
    background-image: url(/fit-woman-training-with-dumbbells.png);
    background-size: 100%;
    background-repeat: no-repeat;
    background-position: center;
}

.logo {
    width: 110px;
    height: 125px;

    position: absolute;
    left: 905px;
    right: 905px;
    top: 130px;
}

.entry {
    position: absolute;
    width: 1180px;
    height: 235px;
    left: 370px;
    top: 360px;
}

.entry p {
    width: 1180px;
    height: 65px;
    margin: 0 0 14px 0;
    font-size: 55px;
    font-weight: bold;
    line-height: 65px;
    text-transform: uppercase;
    color: #FFFFFF;
    text-align: center;

}

.entry p span {
    color: #95E82C;
    font-size: 55px;
}

.entry span {
    width: 1180px;
    height: 35px;
    left: 370px;
    top: 439px;

    font-family: 'Jost';
    font-size: 30px;
    line-height: 35px;

    text-align: center;
    color: #FFFFFF;
}

.entry button {
    position: absolute;
    width: 210px;
    height: 60px;
    left: 485px;
    right: 485px;
    top: 180px;

    padding: 19px 50px 18px 50px;
    background-color: #95E82C;
    border: none;

    font-weight: 700;
    font-size: 16px;
    line-height: 23px;
    text-transform: uppercase;
    color: #000000;
    transition: background-color 150ms;
    cursor: pointer;
}

.entry button:hover {
    background-color: #F6F6F6;
}

@media (width <=768px) {}

@media (width <=340px) {}
</style>