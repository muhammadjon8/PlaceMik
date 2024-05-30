<template>
  <div>
    <div class="flex justify-between w-[65%] ml-[30%] py-2">
      <div class=" text-[10px]">
        <select id="category">
          <option value="Покупателям">Покупателям</option>
        </select>
        <select name="category" id="">
          <option value="Поставщикам">Поставщикам</option>
        </select>
        <select name="category" id="">
          <option value="Частые вопросы">Частые вопросы</option>
        </select>
      </div>
      <div class="flex divide-x-2 divide-black items-center">
        <img src="../assets/Flag Ru.png" alt="" class="px-2 h-[10px]" />
        <p class="px-2 text-[10px]">Русский</p>
        <select name="valyuta" id="valyuta" class="px-2 text-[10px]">
          <option value="₽">₽</option>
          <option value="$">$</option>
          <option value="som">S</option>
        </select>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped></style>
