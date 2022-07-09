<template>
  <div>
    <nav class="flex items-center justify-between flex-wrap bg-teal-500 p-6 rounded">
      <div class="block lg:hidden">
        <button @click="showMenu = !showMenu"
                class="flex items-center px-3 py-2 border rounded text-teal-200 border-teal-400 hover:border-white">
          <svg xmlns="http://www.w3.org/2000/svg" class="h-7 w-7" viewBox="0 0 20 20" fill="currentColor">
            <path fill-rule="evenodd"
                  d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 15a1 1 0 011-1h6a1 1 0 110 2H4a1 1 0 01-1-1z"
                  clip-rule="evenodd"/>
          </svg>
        </button>
      </div>
      <div class="flex items-center flex-shrink-0 text-white mr-6">
        <span class="text-xl font-semibold">مای شاپ</span>
      </div>
      <div class="w-full block flex-grow lg:flex lg:items-center lg:w-auto" v-show="showMenu">
        <div class="text-sm lg:flex-grow">
          <a href="#" class="block mt-4 lg:inline-block lg:mt-0 text-teal-200 hover:text-white mx-4">خانه</a>
          <a href="#" class="block mt-4 lg:inline-block lg:mt-0 text-teal-200 hover:text-white mx-4">درباره ما</a>
          <a href="#" class="block mt-4 lg:inline-block lg:mt-0 text-teal-200 hover:text-white mx-4">ناوبار یک</a>
        </div>
      </div>
      <div>
        <a href="#"
           class="inline-block text-sm px-4 py-2 leading-none border rounded text-white hover:border-transparent hover:text-teal-500 hover:bg-white mt-4 lg:mt-0">Download</a>
      </div>
    </nav>

    <!--    sub navbar-->
    <div>
      <img class="w-full h-96" src="https://faradars.org/next/imgs/banner.jpg" alt="">
    </div>
    <!--    end sub navbar-->

    <div class="mt-9 text-center">
      <span class="font-bold text-base">موضوعات و محورهای آموزشی منتخب</span>
      <div class="mt-5 mx-12 lg:mx-36">
        <div class="grid grid-cols-4 lg:grid-cols-8 gap-4 text-base">
          <div class="flex flex-col mb-2 hover:border-gray-800 hover:bg-gray-100">
            <img class="w-12 h-12 mr-3" src="https://faradars.org/next/svg/collections/programming.svg" alt="">
            <span class="mt-3 text-right">برنامه نویسی</span>
          </div>

          <div class="flex flex-col hover:border-gray-800 hover:bg-gray-100">
            <img class="w-12 h-12 mr-3" src="https://faradars.org/next/svg/collections/exchange.svg" alt="">
            <span class="mt-3 text-right">بورس و بازارسهام</span>
          </div>

          <div class="flex flex-col hover:border-gray-800 hover:bg-gray-100">
            <img class="w-12 h-12 mr-3" src="https://faradars.org/next/svg/collections/business.svg" alt="">
            <span class="mt-3 text-right">استارپاپ و کسب وکار</span>
          </div>

          <div class="flex flex-col hover:border-gray-800 hover:bg-gray-100">
            <img class="w-12 h-12 mr-3" src="https://faradars.org/next/svg/collections/computer.svg" alt="">
            <span class="mt-3 text-right">مهندسی نرم افزار</span>
          </div>

          <div class="flex flex-col hover:border-gray-800 hover:bg-gray-100">
            <img class="w-12 h-12 mr-3" src="https://faradars.org/next/svg/collections/ai.svg" alt="">
            <span class="mt-3 text-right">هوش مصنوعی</span>
          </div>

          <div class="flex flex-col hover:border-gray-800 hover:bg-gray-100">
            <img class="w-12 h-12 mr-3" src="https://faradars.org/next/svg/collections/math.svg" alt="">
            <span class="mt-3 text-right">ریاضیات</span>
          </div>

          <div class="flex flex-col hover:border-gray-800 hover:bg-gray-100">
            <img class="w-12 h-12 mr-3" src="https://faradars.org/next/svg/collections/humanities.svg" alt="">
            <span class="mt-3 text-right">علوم انسانی</span>
          </div>

          <div class="flex flex-col hover:border-gray-800 hover:bg-gray-100">
            <img class="w-12 h-12 mr-3" src="https://faradars.org/next/svg/collections/art.svg" alt="">
            <span class="mt-3 text-right">هنر</span>
          </div>

          <div class="flex flex-col hover:border-gray-800 hover:bg-gray-100">
            <img class="w-12 h-12 mr-3" src="https://faradars.org/next/svg/collections/robotics.svg" alt="">
            <span class="mt-3 text-right">رباتیک</span>
          </div>

          <div class="flex flex-col hover:border-gray-800 hover:bg-gray-100">
            <img class="w-12 h-12 mr-3" src="https://faradars.org/next/svg/collections/statistics.svg" alt="">
            <span class="mt-3 text-right">آمار و داده کاوی</span>
          </div>

          <div class="flex flex-col hover:border-gray-800 hover:bg-gray-100">
            <img class="w-12 h-12 mr-3" src="https://faradars.org/next/svg/collections/matlab.svg" alt="">
            <span class="mt-3 text-right">متلب و سیمیولینک</span>
          </div>

          <div class="flex flex-col hover:border-gray-800 hover:bg-gray-100">
            <img class="w-12 h-12 mr-3" src="https://faradars.org/next/svg/collections/management.svg" alt="">
            <span class="mt-3 text-right">مدیریت</span>
          </div>

          <div class="flex flex-col hover:border-gray-800 hover:bg-gray-100">
            <img class="w-12 h-12 mr-3" src="https://faradars.org/next/svg/collections/englishLearning.svg" alt="">
            <span class="mt-3 text-right">زبان انگلیسی</span>
          </div>

          <div class="flex flex-col hover:border-gray-800 hover:bg-gray-100">
            <img class="w-12 h-12 mr-3" src="https://faradars.org/next/svg/collections/electrical.svg" alt="">
            <span class="mt-3 text-right">مهندسی برق</span>
          </div>

          <div class="flex flex-col hover:border-gray-800 hover:bg-gray-100">
            <img class="w-12 h-12 mr-3" src="https://faradars.org/next/svg/collections/mechanical.svg" alt="">
            <span class="mt-3 text-right">مهندسی مکانیک</span>
          </div>

          <div class="flex flex-col hover:border-gray-800 hover:bg-gray-100">
            <img class="w-12 h-12 mr-3" src="https://faradars.org/next/svg/collections/civil.svg" alt="">
            <span class="mt-3 text-right">مهندسی عمران</span>
          </div>

          <div class="flex flex-col hover:border-gray-800 hover:bg-gray-100">
            <img class="w-12 h-12 mr-3" src="https://faradars.org/next/svg/collections/architect.svg" alt="">
            <span class="mt-3 text-right">مهندسی معماری</span>
          </div>

          <div class="flex flex-col hover:border-gray-800 hover:bg-gray-100">
            <img class="w-12 h-12 mr-3" src="https://faradars.org/next/svg/collections/control.svg" alt="">
            <span class="mt-3 text-right">مهندسی کنترل</span>
          </div>

          <div class="flex flex-col hover:border-gray-800 hover:bg-gray-100">
            <img class="w-12 h-12 mr-3" src="https://faradars.org/next/svg/collections/industrial.svg" alt="">
            <span class="mt-3 text-right">مهندسی صنایع</span>
          </div>

          <div class="flex flex-col hover:border-gray-800 hover:bg-gray-100">
            <img class="w-12 h-12 mr-3" src="https://faradars.org/next/svg/collections/academicWriting.svg" alt="">
            <span class="mt-3 text-right">نگارش آکادمیک</span>
          </div>

          <div class="flex flex-col hover:border-gray-800 hover:bg-gray-100">
            <img class="w-12 h-12 mr-3" src="https://faradars.org/next/svg/collections/excel.svg" alt="">
            <span class="mt-3 text-right">اکسل</span>
          </div>

          <div class="flex flex-col hover:border-gray-800 hover:bg-gray-100">
            <img class="w-12 h-12 mr-3" src="https://faradars.org/next/svg/collections/graphics.svg" alt="">
            <span class="mt-3 text-right">طراحی گرافیک</span>
          </div>

          <div class="flex flex-col hover:border-gray-800 hover:bg-gray-100">
            <img class="w-12 h-12 mr-3" src="https://faradars.org/next/svg/collections/web.svg" alt="">
            <span class="mt-3 text-right">برنامه نویسی وب</span>
          </div>

          <div class="flex flex-col hover:border-gray-800 hover:bg-gray-100">
            <img class="w-12 h-12 mr-3" src="https://faradars.org/next/svg/collections/wp.svg" alt="">
            <span class="mt-3 text-right">وردپرس</span>
          </div>
        </div>
        <div class="mt-3 mb-3">
          <button class="bg-blue-600 px-3 py-3 text-white rounded">همه آموزش ها</button>
        </div>
      </div>
    </div>

<!--    start items page-->
    <div class="mt-8 mx-8 lg:mx-36 text-base">
      <span class="font-bold">آموزش های پرمخاطب</span>
    </div>


<!--    end items page-->
  </div>
</template>


<script>
export default {
  data() {
    return {
      showMenu: true,
    }
  }
}
</script>