<template>
    <div class="reviews">
        <div class="reviews-flex-container">
            <p class="reviews__title">отзывы наших клиентов</p>
            <div class="reviews-information-block">
                <div v-for="review in reviews" class="review__card">
                    <div class="review__rating">{{ review.rating }}</div>
                    <div class="review__text">{{ review.review }}</div>
                    <div class="review__author">
                        <img :src="review.author.img" :alt="review.author.name">
                        <div class="author__bio">
                            <span class="bio__name">{{ review.author.name }}</span>
                            <span class="bio__age">{{ review.author.age }} лет</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "reviews",
    data() {
        return {
            reviews: [
                {
                    rating: '☆ ☆ ☆ ☆ ☆',
                    review: 'Посещаю клуб три раза в неделю. Была на групповых занятиях по аэробике. Мне понравился тренер, он очень динамичный, все объясняет, показывает, заводной. Нравится интерьер, очень гостеприимный персонал, вежливый, всегда чисто в зале, тренажеры новые.',
                    author: {
                        img: 'екатерина.png',
                        name: 'Екатерина',
                        age: 28,
                    }
                },
                {
                    rating: '☆ ☆ ☆ ☆ ☆',
                    review: 'Хорошо продуманная логистика, большая парковка, дизайн реcепшина отличный, электронные браслеты облегчают использование клуба, тренажёрные залы по многим спорт направлениям, квалифицированный персонал, доброжилательная атмосфера, отличные бассейны, разнообразие в программах',
                    author: {
                        img: 'ярослав.png',
                        name: 'Ярослав',
                        age: 36,
                    }
                },
                {
                    rating: '☆ ☆ ☆ ☆ ☆',
                    review: 'Каждый день хожу на кардио и силовые, очень нравится! Все качественно, внешний вид хороший, приятно заниматься. Эффект виден, начала худеть.',
                    author: {
                        img: 'мария.png',
                        name: 'Мария',
                        age: 25,
                    }
                },
            ]
        }
    }
}
</script>

<style scoped>
.reviews {
    position: absolute;
    left: 0px;
    top: 3025px;

    width: 1920px;
    height: 685px;
    padding: 100px 0 90px 0;
    box-sizing: border-box;

    background-color: #F4F4F4;
}

.reviews-flex-container {
    position: absolute;
    left: 370px;

    width: 1180px;
    height: 570px;
}

.reviews__title {
    width: 1180px;
    height: 45px;
    margin: 0;

    font-weight: 700;
    font-size: 35px;
    line-height: 45px;

    text-align: center;
    text-transform: uppercase;
}

.reviews-information-block {
    position: absolute;
    top: 105px;

    width: 1180px;

    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    vertical-align: top;
    gap: 20px;
}

.review__card {
    width: 380px;
    height: fit-content;
    padding: 30px;
    box-sizing: border-box;

    display: flex;
    flex-direction: column;

    position: relative;

    cursor: pointer;
    background-color: #FFFFFF;
}

.review__rating {
    height: 18px;
    font-weight: 900;
    font-size: 18px;
    color: #95E82C;
    text-align: left;
}

.review__text {
    font-weight: 400;
    font-size: 16px;
    line-height: 24px;
    text-align: left;
    margin: 23px 0 36px;

    color: #444444;
}

.review__author {
    display: flex;
    flex-direction: row;

}

.review__author img {
    width: 60px;
    height: 60px;
    border-radius: 50%;
}

.author__bio {
    position: relative;
    display: flex;
    flex-direction: column;

    margin-left: 20px;
    text-align: left;
}

.bio__name {
    position: absolute;
    top: 6px;

    width: 250px;
    height: 24px;
    font-weight: 500;
    font-size: 16px;
    line-height: 24px;

    color: #000000;
}

.bio__age {
    position: absolute;
    top: 30px;

    width: 250px;
    height: 24px;
    font-weight: 400;
    font-size: 14px;
    line-height: 24px;

    color: #999999;
}

@media (width <=768px) {}

@media (width <=340px) {}
</style>