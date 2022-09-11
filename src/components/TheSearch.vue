<template>
  <div class="flex items-center mt-10 justify-start ml-20">
    <div
      class="flex items-center pl-5 border border-sky-500 rounded-xl w-1/2 h-11 bg-gray-50 font-['Gilroy-Regular']"
    >
      <input
        style="outline: none; border: none;"
        type="text"
        placeholder="Какой товар вы ищете?"
        class="w-full h-full bg-gray-50"
      />
      <a href="#"><svg
        class="mr-5"
        width="20"
        height="20"
        viewBox="0 0 20 20"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M8 2C4.68629 2 2 4.68629 2 8C2 11.3137 4.68629 14 8 14C11.3137 14 14 11.3137 14 8C14 4.68629 11.3137 2 8 2ZM0 8C0 3.58172 3.58172 0 8 0C12.4183 0 16 3.58172 16 8C16 9.84871 15.3729 11.551 14.3199 12.9056L19.7071 18.2929C20.0976 18.6834 20.0976 19.3166 19.7071 19.7071C19.3166 20.0976 18.6834 20.0976 18.2929 19.7071L12.9056 14.3199C11.551 15.3729 9.84871 16 8 16C3.58172 16 0 12.4183 0 8Z"
          fill="#139DEB"
        />
      </svg></a>
    </div>
    <button
      onclick="location.href='#'"
      class="font-['Gilroy-SemiBold'] hover:bg-sky-700 hover:border-sky-700 transition duration-500 ml-6 flex items-center pl-5 pr-5 pt-2 pb-2 bg-sky-500 border-2 border-sky-500 rounded-xl text-white"
    >
      Профиль
      <svg
        style="margin-left: 15px;"
        width="18"
        height="20"
        viewBox="0 0 18 20"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M9 2C6.79086 2 5 3.79086 5 6C5 8.20914 6.79086 10 9 10C11.2091 10 13 8.20914 13 6C13 3.79086 11.2091 2 9 2ZM3 6C3 2.68629 5.68629 0 9 0C12.3137 0 15 2.68629 15 6C15 9.31371 12.3137 12 9 12C5.68629 12 3 9.31371 3 6ZM5 16C3.34315 16 2 17.3431 2 19C2 19.5523 1.55228 20 1 20C0.447715 20 0 19.5523 0 19C0 16.2386 2.23858 14 5 14H13C15.7614 14 18 16.2386 18 19C18 19.5523 17.5523 20 17 20C16.4477 20 16 19.5523 16 19C16 17.3431 14.6569 16 13 16H5Z"
          fill="white"
        />
      </svg>
    </button>
    <button
      onclick="location.href='#'"
      class="font-['Gilroy-SemiBold'] hover:bg-gray-200 hover:border-gray-200 transition duration-500 ml-6 flex items-center pl-5 pr-5 pt-2 pb-2 border-2 border-sky-500 rounded-xl text-sky-500 font-semibold"
    >
      2600
      <svg
        style="margin-left: 15px;"
        width="22"
        height="16"
        viewBox="0 0 22 16"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M11 0C17.075 0 22 2.686 22 6V10C22 13.314 17.075 16 11 16C5.033 16 0.176 13.409 0.005 10.177L0 10V6C0 2.686 4.925 0 11 0ZM11 12C7.28 12 3.99 10.993 2 9.45V10C2 11.882 5.883 14 11 14C16.01 14 19.838 11.97 19.995 10.118L20 10L20.001 9.45C18.011 10.992 14.721 12 11 12ZM11 2C5.883 2 2 4.118 2 6C2 7.882 5.883 10 11 10C16.117 10 20 7.882 20 6C20 4.118 16.117 2 11 2Z"
          fill="#139DEB"
        />
      </svg>
    </button>
    <button
      onclick="location.href='#'"
      class="hover:bg-sky-700 hover:border-sky-700 transition duration-500 ml-6 flex items-center pl-4 pr-4 pt-3 pb-3 bg-sky-500 border-sky-500 rounded-xl text-white"
    >
      <svg
        width="20"
        height="20"
        viewBox="0 0 20 20"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M2.1421 2.00002L4.00913 14.1357C4.02271 14.2359 4.05113 14.3313 4.0921 14.4198C4.21543 14.6861 4.45246 14.889 4.74088 14.9661C4.82899 14.9898 4.92133 15.0016 5.01578 15H16C16.4416 15 16.8309 14.7103 16.9578 14.2874L19.9578 4.28736C20.0487 3.98459 19.991 3.65669 19.8023 3.40308C19.6136 3.14948 19.3161 3.00002 19 3.00002H4.31948L3.99058 0.862207C3.97826 0.772825 3.95413 0.687212 3.91981 0.606996C3.85751 0.46092 3.76213 0.334387 3.64429 0.235207C3.53497 0.143016 3.40561 0.0738391 3.26367 0.0351428C3.17434 0.0106786 3.0806 -0.00157508 2.9847 1.52593e-05H1C0.447715 1.52593e-05 0 0.44773 0 1.00002C0 1.5523 0.447715 2.00002 1 2.00002H2.1421ZM5.85794 13L4.62717 5.00002H17.656L15.256 13H5.85794Z"
          fill="white"
        />
        <path
          d="M8 18C8 19.1046 7.10457 20 6 20C4.89543 20 4 19.1046 4 18C4 16.8954 4.89543 16 6 16C7.10457 16 8 16.8954 8 18Z"
          fill="white"
        />
        <path
          d="M17 18C17 19.1046 16.1046 20 15 20C13.8954 20 13 19.1046 13 18C13 16.8954 13.8954 16 15 16C16.1046 16 17 16.8954 17 18Z"
          fill="white"
        />
      </svg>
    </button>
  </div>
</template>
