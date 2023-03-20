<template>
  <div class="navigation">
    <div class="networks">
      <i class="fa-brands fa-instagram"></i>
      <i class="fa-brands fa-vk"></i>
      <i class="fa-brands fa-telegram"></i>
    </div>
    <div class="menu">
      <span>УСЛУГИ</span>
      <span>О КЛУБЕ</span>
      <span>ТРЕНЕРЫ</span>
      <span>ОТЗЫВЫ</span>
      <span>НОВОСТИ</span>
      <span>КОНТАКТЫ</span>
    </div>
    <div class="call">
      <i class="fa-solid fa-phone-volume"></i>
      <span class="phone-number">8 800 555 30 50</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "navigation",
}
</script>

<style scoped>
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

.networks {
  position: absolute;
  width: 100px;
  height: 20px;
  left: 370px;
  top: 50px;

  display: flex;
  flex-direction: row;
  gap: 20px;

  color: #95E82C;
}

.call {
  position: absolute;
  width: 165px;
  height: 20px;
  left: 1385px;
  top: 50px;

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

.menu {
  display: flex;
  flex-direction: row;
  align-items: flex-start;
  gap: 50px;

  position: absolute;
  width: 626px;
  height: 20px;
  left: 647px;
  top: 50px;

  font-weight: 500;
  font-size: 14px;
  color: #FFFFFF;
}

.menu span {
  transition: background-color 150ms;
  cursor: pointer;
}

.menu span:hover {
  color: #95E82C;
}

@media (width <=768px) {}

@media (width <=340px) {}
</style>