<script setup>
import { ref } from "vue";
import boyImage from "../assets/boy.png";
import phone1 from "../assets/phone1.png";
import hat from "../assets/hat.png";

const card = ref([
  {
    photo: boyImage,
    price: "1 999 ₽",
    sale: "2 499 ₽",
    description: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
    star: 4.9,
    comments: 14,
    model: "MARPLE",
  },
  {
    photo: phone1,
    price: "1 999 ₽",
    sale: "2 499 ₽",
    description: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
    star: 4.9,
    comments: 14,
    model: "MARPLE",
  },
  {
    photo: hat,
    price: "1 999 ₽",
    sale: "2 499 ₽",
    description: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
    star: 4.9,
    comments: 14,
    model: "MARPLE",
  },
  {
    photo: boyImage,
    price: "1 999 ₽",
    sale: "2 499 ₽",
    description: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
    star: 4.9,
    comments: 14,
    model: "MARPLE",
  },
  {
    photo: phone1,
    price: "1 999 ₽",
    sale: "2 499 ₽",
    description: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
    star: 4.9,
    comments: 14,
    model: "MARPLE",
  },
  {
    photo: hat,
    price: "1 999 ₽",
    sale: "2 499 ₽",
    description: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
    star: 4.9,
    comments: 14,
    model: "MARPLE",
  },
  {
    photo: phone1,
    price: "1 999 ₽",
    sale: "2 499 ₽",
    description: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
    star: 4.9,
    comments: 14,
    model: "MARPLE",
  },
  {
    photo: boyImage,
    price: "1 999 ₽",
    sale: "2 499 ₽",
    description: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
    star: 4.9,
    comments: 14,
    model: "MARPLE",
  },
  {
    photo: hat,
    price: "1 999 ₽",
    sale: "2 499 ₽",
    description: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
    star: 4.9,
    comments: 14,
    model: "MARPLE",
  },
  {
    photo: phone1,
    price: "1 999 ₽",
    sale: "2 499 ₽",
    description: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
    star: 4.9,
    comments: 14,
    model: "MARPLE",
  },
  {
    photo: boyImage,
    price: "1 999 ₽",
    sale: "2 499 ₽",
    description: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
    star: 4.9,
    comments: 14,
    model: "MARPLE",
  },
  {
    photo: phone1,
    price: "1 999 ₽",
    sale: "2 499 ₽",
    description: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
    star: 4.9,
    comments: 14,
    model: "MARPLE",
  },
]);
</script>

<template>
  <div>
    <div class="container">
      <h2 class="text-[28px] font-normal">Успей купить</h2>
      <div class="grid grid-cols-6 gap-5">
        <div v-for="(item, index) in card" :key="index" class="w-full relative">
          <div
            class="group bg-white p-4 border rounded-md shadow-3xl w-full h-auto hover:absolute top-0 left-0 z-30  hover:scale-105 duration-300"
          >
            <img :src="item.photo" alt="" />
            <div class="flex items-center gap-4">
              <p class="text-[14px] font-medium text-red-500">
                {{ item.price }}
              </p>
              <p class="text-[10px] text-[#4646468C] line-through">
                {{ item.sale }}
              </p>
            </div>
            <div class="hidden group-hover:block">
              <div class="flex items-center gap-4">
                <div class="flex items-center gap-1">
                  <p class="text-[12px]">{{ item.star }}</p>
                  <img
                    src="../assets/star.png"
                    alt=""
                    class="w-[16px] h-[16px]"
                  />
                </div>
                <p class="text-[12px]">{{ item.comments }} отзывов</p>
              </div>
              <p class="text-[12px] font-medium">{{ item.model }}</p>
            </div>
            <p class="text-[12px] leading-3 font-light">
              {{ item.description }}
            </p>

            <button
              class="group-hover:block hidden py-2 mt-3 bg-gradient-to-r from-purple-500 to-pink-500 text-white w-full"
            >
              В корзину
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="css" scoped></style>
