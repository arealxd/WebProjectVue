<template>
  <header class="flex mt-5 items-center">
    <div class="flex items-center w-1/2">
      <div class="font-['Gilroy-SemiBold']">
        <button
          onclick="location.href='#'"
          class="hover:bg-red-500 transition duration-500 hover:text-white ml-20 pl-5 pr-5 pt-1 pb-1 border border-red-500 rounded-xl text-red-500 font-semibold"
        >
          Акции
        </button>
      </div>
      <div class="font-['Gilroy-SemiBold']">
        <button
          onclick="location.href='#'"
          class="hover:bg-sky-500 transition duration-500 hover:text-white ml-10 pl-5 pr-5 pt-1 pb-1 border border-sky-500 rounded-xl text-sky-500 font-semibold"
        >
          Сеты
        </button>
      </div>
      <div class="font-['Gilroy-Light']">
        <button
          onclick="location.href='#'"
          class="hover:underline underline-offset-8 ml-10"
        >
          Новости
        </button>
      </div>
      <div class="font-['Gilroy-Light']">
        <button
          onclick="location.href='#'"
          class="hover:underline underline-offset-8 ml-10"
        >
          Доставка
        </button>
      </div>
      <div class="font-['Gilroy-Light']">
        <button
          onclick="location.href='#'"
          class="hover:underline underline-offset-8 ml-10"
        >
          Условия
        </button>
      </div>
    </div>
    <div class="flex w-1/2 justify-end mr-20 font-['Gilroy-Light']">
      <div>
        <select style="width: 80px; outline: none;">
          <option>Актобе</option>
          <option>Астана</option>
          <option>Алматы</option>
        </select>
      </div>
      <div>
        <select class="ml-6" style="outline: none;">
          <option>RU</option>
          <option>EN</option>
          <option>KZ</option>
        </select>
      </div>
    </div>
  </header>
</template>
