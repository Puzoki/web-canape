<template>
    <div class="coaches">
        <div class="coaches-flex-container">
            <p class="coaches__title">наши тренеры</p>
            <div class="coaches-information-block">
                <div v-for="coache in coaches" class="coache__card">
                    <div class="card__bio">
                        <span class="bio__name">{{ coache.name }}</span>
                        <span class="bio__experience">Стаж {{ coache.experience }} лет</span>
                    </div>
                    <img :src="coache.img" :alt="coache.name">
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "coaches",
    data() {
        return {
            coaches: [
                {
                    img: 'быстров.png',
                    name: 'Максим Быстров',
                    experience: 12,
                },
                {
                    img: 'адамов.png',
                    name: 'Рустам Адамов',
                    experience: 13,
                },
                {
                    img: 'попова.png',
                    name: 'Мария Попова',
                    experience: 10,
                },
                {
                    img: 'киреева.png',
                    name: 'Эльвира Киреева',
                    experience: 8,
                },
                {
                    img: 'шмурнов.png',
                    name: 'Глеб Шмурнов',
                    experience: 7,
                },
                {
                    img: 'шарифова.png',
                    name: 'Зарина Шарифова',
                    experience: 11,
                },
                {
                    img: 'смирнов.png',
                    name: 'Алексей Смирнов',
                    experience: 5,
                },
                {
                    img: 'шатова.png',
                    name: 'Ирина Шатова',
                    experience: 6,
                },
                {
                    img: 'войнов.png',
                    name: 'Даниил Войнов',
                    experience: 5,
                },
            ]
        }
    }
}
</script>

<style scoped>
.coaches {
    position: absolute;
    top: 2320px;

    width: 1920px;
    height: 705px;
    background-color: #FFFFFF;
}

.coaches-flex-container {
    position: absolute;
    left: 370px;

    width: 1180px;
    height: 705px;
}

.coaches__title {
    width: 1180px;
    height: 45px;

    position: absolute;
    top: 100px;
    margin: 0;

    font-weight: 700;
    font-size: 35px;
    line-height: 45px;

    text-align: center;
    text-transform: uppercase;
}

.coaches-information-block {
    position: absolute;
    top: 205px;

    width: 1180px;
    height: 400px;

    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    gap: 20px;
}

.coache__card {
    width: 380px;
    height: 120px;
    box-sizing: border-box;
    border: solid 1px #DDDDDD;
    border-left: solid 6px #95E82C;

    display: flex;
    flex-direction: row;

    position: relative;
    overflow: hidden;

    cursor: pointer;
    transition: border 150ms;
}

.coache__card:hover {
    border: solid 1px #bbbbbb;
    border-left: solid 6px #95E82C;
}

.coache__card img {
    position: absolute;
    right: 0;
}

.card__bio {
    display: flex;
    flex-direction: column;

    text-align: left;
}

.bio__name {
    position: absolute;
    left: 34px;
    top: 30px;

    width: 200px;
    height: 24px;

    font-weight: 500;
    font-size: 20px;
    line-height: 24px;
}

.bio__experience {
    position: absolute;
    left: 34px;
    top: 71px;

    width: 200px;
    height: 24px;

    font-weight: 400;
    font-size: 14px;
    line-height: 24px;

    color: #999999;
}

@media (width <=768px) {}

@media (width <=340px) {}
</style>