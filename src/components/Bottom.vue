<template>
    <div class="footer">
        <img src="/logo.svg" alt="logo">
        <div class="menu">
            <span>УСЛУГИ</span>
            <span>О КЛУБЕ</span>
            <span>ТРЕНЕРЫ</span>
            <span>ОТЗЫВЫ</span>
            <span>НОВОСТИ</span>
            <span>КОНТАКТЫ</span>
        </div>
        <div class="contacts">
            <div class="call">
                <i class="fa-solid fa-phone-volume"></i>
                <span class="phone-number">8 800 555 30 50</span>
            </div>
            <i class="fa-brands fa-instagram"></i>
            <i class="fa-brands fa-vk"></i>
            <i class="fa-brands fa-telegram"></i>
        </div>
        <button>записаться</button>
        <span class="copyright">© Train Hard 2022</span>
        <span class="privacy">Политика конфиденциальности</span>
        <span class="web-canape">Разработка и маркетинг WebCanape</span>
    </div>
</template>

<script>
export default {
    name: "bottom",
}
</script>

<style scoped>
.footer {
    position: absolute;
    top: 4400px;

    width: 1920px;
    height: 300px;

    background-color: #000000;
}

img {
    position: absolute;
    top: 79px;
    left: 370px;

    height: 68px;
    width: 60px;
}

.menu {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    align-items: flex-start;
    gap: 20px;

    position: absolute;
    width: 365px;
    height: 60px;
    left: 570px;
    top: 83px;

    font-weight: 500;
    font-size: 14px;
    color: #FFFFFF;
}

.menu span {
    width: 108px;
    height: 20px;
    text-align: left;
    transition: background-color 150ms;
    cursor: pointer;
}

.menu span:hover {
    color: #95E82C;
}

.contacts {
    position: absolute;
    width: 100px;
    height: 20px;
    left: 1100px;
    top: 83px;

    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    gap: 20px;

    color: #95E82C;
}

.call {
    width: 165px;
    height: 20px;

    display: flex;
    flex-direction: row;
    gap: 10px;

    color: #95E82C;
    transition: background-color 150ms;
    cursor: pointer;
}

.call:hover {
    color: #F6F6F6;
}

.phone-number {
    width: 135px;
    height: 20px;
    font-size: 18px;
    font-weight: 400;
    line-height: 20px;
}

.phone-number:hover {
    color: #F6F6F6;
}

i {
    width: 20px;
    height: 20px;
    font-size: 20px;

    transition: background-color 150ms;
    cursor: pointer;
}

i:hover {
    color: #F6F6F6
}

button {
    position: absolute;
    width: 210px;
    height: 60px;
    right: 370px;
    top: 83px;

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

button:hover {
    background-color: #F6F6F6;
}

.copyright {
    position: absolute;
    bottom: 58px;
    left: 370px;

    width: 180px;
    height: 24px;
    font-weight: 400;
    font-size: 14px;
    line-height: 24px;

    color: #666666;
    text-align: left;
    cursor: pointer;
}

.privacy {
    position: absolute;
    bottom: 58px;
    left: 570px;
    font-weight: 400;
    font-size: 14px;
    line-height: 24px;

    width: 280px;
    height: 24px;

    color: #666666;
    text-align: center;
    cursor: pointer;
}

.web-canape {
    position: absolute;
    bottom: 58px;
    right: 370px;

    width: 280px;
    height: 24px;
    font-weight: 400;
    font-size: 14px;
    line-height: 24px;

    color: #666666;
    text-align: right;
    cursor: pointer;
}

@media (width <=768px) {}

@media (width <=340px) {}
</style>