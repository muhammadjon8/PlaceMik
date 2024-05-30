<script setup></script>

<template>
  <div>
    <div class="container py-3">
      <div class="flex items-center justify-between">
        <div class="flex gap-4">
          <div
            class="hamburger w-[77px] h-[77px] flex items-center justify-center"
          >
            <img src="../assets/men.png" alt="" />
          </div>
          <div class="w-[170px]">
            <img src="../assets/logo.png" alt="" />
            <p class="text-[10px]">Товары из Кореи от производителя</p>
          </div>
        </div>
        <div
          class="navbar__input flex w-[750px] h-[46px] border border-red-200 py-1 px-2"
        >
          <select id="search_option" class="h-[100%] w-[96px] bg-[#0000001F]">
            <option value="Везде">Везде</option>
          </select>
          <input type="text" class="w-[100%] border-none outline-none px-2" />
          <img src="../assets/search.svg" alt="" />
        </div>
        <div class="flex gap-[50px] text-[10px] px-2">
          <div class="flex flex-col items-center">
            <img src="../assets/voyti.png" alt="" />
            <p>Войти</p>
          </div>
          <div class="flex flex-col items-center">
            <img src="../assets/like.png" alt="" />
            <p>Избранное</p>
          </div>
          <div class="flex flex-col items-center">
            <img src="../assets/shop-cart.png" alt="" />
            <p>Корзина</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.hamburger {
  background: linear-gradient(96.78deg, #f64d4d -57.09%, #4d5ef6 101.17%);
}

.navbar__input {
  border-width: 2px; /* Adjust the width as needed */
  border-style: solid;
  border-image: linear-gradient(96.78deg, #f64d4d -57.09%, #4d5ef6 101.17%);
  border-image-slice: 1;
}
</style>
