<template>
    <div v-for="(products, index) in data" :key="products.id" class="-mb-20">
        <div class="flex mt-28 justify-between mx-20">
            <h2 class="font-bold text-3xl text-gray-800 font-['Gilroy-Bold']">{{ index }}</h2>
            <div class="flex">
                <a href="#"><svg class="fill-white hover:fill-gray-200 transition duration-300" width="40" height="40" viewBox="0 0 40 40" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <circle cx="20" cy="20" r="19.5" transform="rotate(-180 20 20)" stroke="#DFDFDF"/>
                    <path d="M22.447 14.2511C22.7399 14.5858 22.7399 15.1285 22.447 15.4632L18.4773 20L22.447 24.5368C22.7399 24.8715 22.7399 25.4142 22.447 25.7489C22.1541 26.0837 21.6793 26.0837 21.3864 25.7489L16.8864 20.6061C16.5935 20.2714 16.5935 19.7286 16.8864 19.3939L21.3864 14.2511C21.6793 13.9163 22.1541 13.9163 22.447 14.2511Z" fill="#139DEB"/>
                </svg></a>
                <div class="ml-4"></div>
                <a href="#"><svg class="fill-white hover:fill-gray-200 transition duration-300" width="40" height="40" viewBox="0 0 40 40" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <circle cx="20" cy="20" r="19.5" stroke="#DFDFDF"/>
                    <path d="M17.553 25.7489C17.2601 25.4142 17.2601 24.8715 17.553 24.5368L21.5226 20L17.553 15.4632C17.2601 15.1285 17.2601 14.5858 17.553 14.251C17.8459 13.9163 18.3207 13.9163 18.6136 14.251L23.1136 19.3939C23.4065 19.7286 23.4065 20.2714 23.1136 20.6061L18.6136 25.7489C18.3207 26.0837 17.8459 26.0837 17.553 25.7489Z" fill="#139DEB"/>
                </svg></a>
            </div> 
        </div>
        <div class="flex mt-6 justify-between mx-20 font-['Gilroy-Regular'] relative">
            <div v-for="product in products" :key="product.name" class="relative border border-gray-300 rounded-lg p-3 mr-5">
                <div v-if="product.new">
                    <p v-if="product.hit" class="bg-[#00AFC7] text-white text-lg pl-4 -ml-3 pt-1 pb-1.5 mt-1 pr-4 rounded-r-lg absolute">Хит</p>
                    <p v-if="product.new" class="bg-[#00AFC7] text-white text-lg pl-4 -ml-3 pt-1 pb-1.5 mt-1 pr-4 rounded-r-lg absolute">Новинка</p><br><br>
                    <p v-if="product.sale" class="bg-[#F83C3C] text-white text-lg pl-4 -ml-3 pt-1 pb-1.5 mt-[1px] pr-4 rounded-r-lg absolute">Акция</p><br><br>
                    <p v-if="product.percent !=0" class="bg-[#F83C3C] text-white text-lg pl-4 -ml-3 pt-1 pb-1.5 -mt-[2px] pr-4 rounded-r-lg absolute">{{ product.percent }}%</p>
                    <p v-if="product.basket" class="flex items-center bg-white text-gray-400 text-sm px-3 py-2 rounded-l-lg border absolute right-0 top-4"><svg class="mr-2" width="18" height="18" viewBox="0 0 18 18" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M2.45174 2.33329L4.0076 12.4463C4.01892 12.5298 4.0426 12.6094 4.07674 12.6831C4.17951 12.905 4.37704 13.0741 4.61739 13.1384C4.69081 13.1581 4.76777 13.168 4.84647 13.1666H14C14.368 13.1666 14.6924 12.9252 14.7982 12.5727L17.2982 4.23941C17.3739 3.9871 17.3258 3.71385 17.1686 3.50251C17.0113 3.29117 16.7634 3.16662 16.5 3.16662H4.26622L3.99214 1.38511C3.98187 1.31063 3.96176 1.23928 3.93316 1.17244C3.88125 1.05071 3.80176 0.945261 3.70357 0.862611C3.61247 0.785785 3.50466 0.728138 3.38638 0.695891C3.31194 0.675504 3.23383 0.665293 3.1539 0.666618H1.49999C1.03975 0.666618 0.666656 1.03971 0.666656 1.49995C0.666656 1.96019 1.03975 2.33329 1.49999 2.33329H2.45174ZM5.54827 11.5L4.52263 4.83329H15.38L13.38 11.5H5.54827Z" fill="#9C9C9C"/>
                    <path d="M7.33332 15.6666C7.33332 16.5871 6.58713 17.3333 5.66666 17.3333C4.74618 17.3333 3.99999 16.5871 3.99999 15.6666C3.99999 14.7461 4.74618 14 5.66666 14C6.58713 14 7.33332 14.7461 7.33332 15.6666Z" fill="#9C9C9C"/>
                    <path d="M14.8333 15.6666C14.8333 16.5871 14.0871 17.3333 13.1667 17.3333C12.2462 17.3333 11.5 16.5871 11.5 15.6666C11.5 14.7461 12.2462 14 13.1667 14C14.0871 14 14.8333 14.7461 14.8333 15.6666Z" fill="#9C9C9C"/>
                    </svg>
                    В корзине
                </p>
            </div>
            <div v-else-if="product.hit">
                    <p v-if="product.hit" class="bg-[#00AFC7] text-white text-lg pl-4 -ml-3 pt-1 pb-1.5 mt-1 pr-4 rounded-r-lg mb-10 absolute">Хит</p><br><br> 
                    <p v-if="product.sale" class="bg-[#F83C3C] text-white text-lg pl-4 -ml-3 pt-1 pb-1.5 mt-[1px] pr-4 rounded-r-lg absolute">Акция</p><br><br>
                    <p v-if="product.percent !=0" class="bg-[#F83C3C] text-white text-lg pl-4 -ml-3 pt-1 pb-1.5 -mt-[2px] pr-4 rounded-r-lg absolute">{{ product.percent }}%</p>
                    <p v-if="product.basket" class="flex items-center bg-white text-gray-400 text-sm px-3 py-2 rounded-l-lg border absolute right-0 top-4"><svg class="mr-2" width="18" height="18" viewBox="0 0 18 18" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M2.45174 2.33329L4.0076 12.4463C4.01892 12.5298 4.0426 12.6094 4.07674 12.6831C4.17951 12.905 4.37704 13.0741 4.61739 13.1384C4.69081 13.1581 4.76777 13.168 4.84647 13.1666H14C14.368 13.1666 14.6924 12.9252 14.7982 12.5727L17.2982 4.23941C17.3739 3.9871 17.3258 3.71385 17.1686 3.50251C17.0113 3.29117 16.7634 3.16662 16.5 3.16662H4.26622L3.99214 1.38511C3.98187 1.31063 3.96176 1.23928 3.93316 1.17244C3.88125 1.05071 3.80176 0.945261 3.70357 0.862611C3.61247 0.785785 3.50466 0.728138 3.38638 0.695891C3.31194 0.675504 3.23383 0.665293 3.1539 0.666618H1.49999C1.03975 0.666618 0.666656 1.03971 0.666656 1.49995C0.666656 1.96019 1.03975 2.33329 1.49999 2.33329H2.45174ZM5.54827 11.5L4.52263 4.83329H15.38L13.38 11.5H5.54827Z" fill="#9C9C9C"/>
                    <path d="M7.33332 15.6666C7.33332 16.5871 6.58713 17.3333 5.66666 17.3333C4.74618 17.3333 3.99999 16.5871 3.99999 15.6666C3.99999 14.7461 4.74618 14 5.66666 14C6.58713 14 7.33332 14.7461 7.33332 15.6666Z" fill="#9C9C9C"/>
                    <path d="M14.8333 15.6666C14.8333 16.5871 14.0871 17.3333 13.1667 17.3333C12.2462 17.3333 11.5 16.5871 11.5 15.6666C11.5 14.7461 12.2462 14 13.1667 14C14.0871 14 14.8333 14.7461 14.8333 15.6666Z" fill="#9C9C9C"/>
                    </svg>
                    В корзине
                    </p>
            </div>
            <div v-else>
                    <p v-if="product.hit" class="bg-[#00AFC7] text-white text-lg pl-4 -ml-3 pt-1 pb-1.5 mt-1 pr-4 rounded-r-lg mb-10 absolute">Хит</p> 
                    <p v-if="product.sale" class="bg-[#F83C3C] text-white text-lg pl-4 -ml-3 pt-1 pb-1.5 mt-[1px] pr-4 rounded-r-lg absolute">Акция</p><br><br>
                    <p v-if="product.percent !=0" class="bg-[#F83C3C] text-white text-lg pl-4 -ml-3 pt-1 pb-1.5 -mt-[2px] pr-4 rounded-r-lg absolute">{{ product.percent }}%</p>
                    <p v-if="product.basket" class="flex items-center bg-white text-gray-400 text-sm px-3 py-2 rounded-l-lg border absolute right-0 top-4"><svg class="mr-2" width="18" height="18" viewBox="0 0 18 18" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M2.45174 2.33329L4.0076 12.4463C4.01892 12.5298 4.0426 12.6094 4.07674 12.6831C4.17951 12.905 4.37704 13.0741 4.61739 13.1384C4.69081 13.1581 4.76777 13.168 4.84647 13.1666H14C14.368 13.1666 14.6924 12.9252 14.7982 12.5727L17.2982 4.23941C17.3739 3.9871 17.3258 3.71385 17.1686 3.50251C17.0113 3.29117 16.7634 3.16662 16.5 3.16662H4.26622L3.99214 1.38511C3.98187 1.31063 3.96176 1.23928 3.93316 1.17244C3.88125 1.05071 3.80176 0.945261 3.70357 0.862611C3.61247 0.785785 3.50466 0.728138 3.38638 0.695891C3.31194 0.675504 3.23383 0.665293 3.1539 0.666618H1.49999C1.03975 0.666618 0.666656 1.03971 0.666656 1.49995C0.666656 1.96019 1.03975 2.33329 1.49999 2.33329H2.45174ZM5.54827 11.5L4.52263 4.83329H15.38L13.38 11.5H5.54827Z" fill="#9C9C9C"/>
                    <path d="M7.33332 15.6666C7.33332 16.5871 6.58713 17.3333 5.66666 17.3333C4.74618 17.3333 3.99999 16.5871 3.99999 15.6666C3.99999 14.7461 4.74618 14 5.66666 14C6.58713 14 7.33332 14.7461 7.33332 15.6666Z" fill="#9C9C9C"/>
                    <path d="M14.8333 15.6666C14.8333 16.5871 14.0871 17.3333 13.1667 17.3333C12.2462 17.3333 11.5 16.5871 11.5 15.6666C11.5 14.7461 12.2462 14 13.1667 14C14.0871 14 14.8333 14.7461 14.8333 15.6666Z" fill="#9C9C9C"/>
                    </svg>
                    В корзине
                    </p>
            </div>
                <img class="-mt-10" :src="product.img" alt="juice">
                <p class="ml-2 leading-5 w-[250px]">{{ product.name }}</p>
                <p class="ml-2 text-xs text-gray-500 mt-2 font-['Gilroy-Medium']">Omar Market</p>
                <hr class="mt-2 mb-2">
                <div class="flex justify-between">
                    <p>{{ product.characteristics.volume_name }}</p>
                    <p>{{ product.characteristics.box_name }}</p>
                    <p v-if="product.characteristics.cost != ''" class="text-[#139DEB]">{{product.characteristics.cost_name}}</p>
                </div>
                <div class="flex justify-between mt-3">
                    <p>{{ product.characteristics.volume }}</p>
                    <p class="ml-3">{{ product.characteristics.box }}</p>
                    <div v-show="product.oldPrice != 0" class="-m-3 mt-[0.2px]">
                    <p class="text-right text-xs text-gray-500 line-through mr-3">{{ product.oldPrice }}</p>
                        <p class="text-[#139DEB] -mt-2 mr-3">{{product.characteristics.cost}}</p>
                    </div>
                    <p v-show="product.oldPrice == 0" class="text-[#139DEB]">{{product.characteristics.cost}}</p>
                </div>
                <div class="flex items-center justify-center mt-4 mb-2">
                    <a href="#" class="flex"><p class="text-[#139DEB] font-semibold hover:text-sky-700 transition duration-300">Подробнее</p>
                    <svg class="mt-2.5 ml-1.5" width="13" height="8" viewBox="0 0 13 8" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M0.910749 0.744078C1.23619 0.418641 1.76382 0.418641 2.08926 0.744078L6.5 5.15482L10.9107 0.744078C11.2362 0.418641 11.7638 0.418641 12.0893 0.744078C12.4147 1.06951 12.4147 1.59715 12.0893 1.92259L7.08926 6.92259C6.76382 7.24803 6.23619 7.24803 5.91075 6.92259L0.910749 1.92259C0.585313 1.59715 0.585313 1.06951 0.910749 0.744078Z" fill="#139DEB"/>
                    </svg></a>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import data from "../assets/data.json"
export default {
    name: "Content",
    data() {
        return {
            data
        }
    }
}
</script>