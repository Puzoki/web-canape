<template>
  <div class="promo">
    <div class="networks">
      <div class="networks__icon">
        <i class="fa-brands fa-instagram"></i>
      </div>
      <div class="networks__icon">
        <i class="fa-brands fa-vk"></i>
      </div>
      <div class="networks__icon">
        <i class="fa-brands fa-telegram"></i>
      </div>
    </div>
    <img class="logo" src="/logo.svg" alt="logo">
    <button>записаться</button>
  </div>
</template>

<script>
export default {
  name: "promo",
}
</script>

<style scoped>
.promo {
  position: absolute;
  left: 0;
  top: 2021px;

  width: 1920px;
  height: 299px;

  background-image: url(/muscular-sportsman-training-arms-with-dumbbell.png);
  background-size: 100%;
  background-position: bottom;
}

.networks {
  position: absolute;
  top: 119.5px;
  left: 370px;

  width: 200px;
  height: 60px;
  display: flex;
  flex-direction: row;
  gap: 10px;
}

.networks__icon {
  width: 60px;
  height: 60px;

  padding: 15px;
  box-sizing: border-box;
  background-color: #97E82C;

  transition: background-color 150ms;
  cursor: pointer;
}

.networks__icon:hover {
  background-color: #F6F6F6;
}

i {
  font-size: 30px;
  color: #000000;
}

.logo {
  width: 150px;
  height: 170px;
  position: absolute;
  left: 885px;
  top: 65px;
}

button {
  position: absolute;
  width: 209px;
  height: 60px;
  right: 370px;
  top: 119.5px;
  padding: 19px 49px 18px 50px;
  background-color: #95E82C;
  border: none;
  font-weight: 700;
  font-size: 16px;
  line-height: 23px;

  text-transform: uppercase;
  transition: background-color 150ms;
  cursor: pointer;
}

button:hover {
  background-color: #F6F6F6;
}

@media (width <=768px) {}

@media (width <=340px) {}
</style>