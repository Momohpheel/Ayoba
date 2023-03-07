<template>
  <div class="py-4 hidden lg:block">
      <nav class="flex justify-between items-center px-20 ">
        <ul class="flex items-center gap-8">
          <li class="">
            <router-link to="/home" class="block">
              <img src="@/assets/logo.svg" alt="" class="logo">
            </router-link>
          </li>
        </ul>
        <ul class="flex justify-between gap-6 items-center py-2">
          <li>
            <router-link to="/about" class="text-sm text-current hover:text-army pb-3">About us</router-link>
          </li>
          <li class="cursor-pointer relative" @mouseover="showProduct = true" @mouseleave="showProduct = false">
            <p class="text-sm text-current hover:text-army">Products</p>
            <transition name="slide"> 
              <div v-if="showProduct" class="absolute pt-6 product">
                <div class="bg-white rounded p-6 shadow-md">
                  <p class="text-gray-500">Plans & Cover</p>
                  <ul class="mt-6 grid grid-cols-2 gap-6 productlist">
                    <li>
                      <router-link to="/products/homecontent" class="flex items-start gap-4">
                        <svg width="50" height="50" viewBox="0 0 50 50" fill="none" xmlns="http://www.w3.org/2000/svg">
                          <circle opacity="0.1" cx="24.9685" cy="24.9685" r="24.9685" fill="#219653"/>
                          <path d="M33.3008 23.0191L25.6175 16.034C25.3353 15.7756 24.9665 15.6323 24.5838 15.6323C24.2012 15.6324 23.8324 15.7757 23.5503 16.0342L15.8683 23.019C15.71 23.1631 15.5835 23.3387 15.4969 23.5344C15.4103 23.7302 15.3655 23.9419 15.3653 24.1559V33.0001C15.3609 33.3862 15.4979 33.7606 15.7505 34.0528C15.8944 34.2163 16.0716 34.3472 16.2702 34.4367C16.4688 34.5262 16.6842 34.5722 16.9021 34.5717H21.5081C21.7118 34.5717 21.9072 34.4907 22.0513 34.3467C22.1954 34.2026 22.2763 34.0072 22.2763 33.8034V29.1931C22.2763 28.9894 22.3573 28.794 22.5013 28.6499C22.6454 28.5058 22.8408 28.4249 23.0446 28.4249H26.1176C26.3214 28.4249 26.5168 28.5058 26.6609 28.6499C26.8049 28.794 26.8859 28.9894 26.8859 29.1931V33.8034C26.8859 34.0072 26.9668 34.2026 27.1109 34.3467C27.255 34.4907 27.4504 34.5717 27.6542 34.5717H32.2692C32.5217 34.575 32.7707 34.5136 32.9927 34.3935C33.2378 34.2612 33.4425 34.0651 33.5853 33.826C33.728 33.5869 33.8035 33.3136 33.8036 33.0352V24.156C33.8034 23.9419 33.7586 23.7303 33.672 23.5345C33.5854 23.3388 33.459 23.1632 33.3008 23.0191Z" fill="#219653"/>
                        </svg>
                        <div>
                          <p class="text-darker font-semibold text-base">Home Insurance</p>
                          <p class="mt-2 text-current text-sm">Insure your Item </p>
                        </div>
                      </router-link>
                    </li>
                    <li>
                      <router-link to="/products/health" class="flex items-start gap-4">
                        <svg width="51" height="50" viewBox="0 0 51 50" fill="none" xmlns="http://www.w3.org/2000/svg">
                          <circle opacity="0.1" cx="25.9055" cy="24.9685" r="24.9685" fill="#DD168D"/>
                          <path d="M30.131 16.1336C29.2366 16.132 28.3542 16.3392 27.554 16.7386C26.7538 17.1381 26.0578 17.7187 25.5214 18.4344C24.795 17.4679 23.783 16.7543 22.6287 16.3946C21.4744 16.0348 20.2362 16.0472 19.0893 16.43C17.9424 16.8127 16.9448 17.5464 16.2379 18.5272C15.5309 19.5081 15.1503 20.6864 15.1499 21.8955C15.156 22.812 15.3161 23.721 15.6233 24.5844H19.7325L21.0409 22.6218C21.1111 22.5165 21.2061 22.4302 21.3176 22.3706C21.4291 22.3109 21.5537 22.2796 21.6801 22.2796C21.8066 22.2796 21.9311 22.3109 22.0426 22.3706C22.1541 22.4302 22.2492 22.5165 22.3193 22.6218L24.7532 26.2725L25.6505 24.9266C25.7206 24.8213 25.8157 24.735 25.9272 24.6753C26.0387 24.6157 26.1632 24.5844 26.2897 24.5844H28.5945C28.7982 24.5844 28.9937 24.6654 29.1377 24.8095C29.2818 24.9535 29.3628 25.1489 29.3628 25.3527C29.3628 25.5565 29.2818 25.7519 29.1377 25.8959C28.9937 26.04 28.7982 26.121 28.5945 26.121H26.7008L25.3924 28.0836C25.3222 28.1889 25.2272 28.2752 25.1157 28.3348C25.0042 28.3945 24.8797 28.4257 24.7532 28.4257C24.6267 28.4257 24.5022 28.3945 24.3907 28.3348C24.2792 28.2752 24.1841 28.1889 24.114 28.0836L21.6801 24.4329L20.7828 25.7788C20.7127 25.8841 20.6176 25.9704 20.5061 26.0301C20.3946 26.0897 20.2701 26.121 20.1436 26.121H16.3007C18.8601 30.9044 24.826 34.2946 25.146 34.4739C25.2607 34.5381 25.39 34.5718 25.5214 34.5718C25.6529 34.5718 25.7822 34.5381 25.8968 34.4739C27.6603 33.4411 29.3153 32.2335 30.837 30.8694C34.1919 27.85 35.893 24.8308 35.893 21.8955C35.8912 20.3679 35.2836 18.9033 34.2034 17.8231C33.1232 16.7429 31.6586 16.1353 30.131 16.1336Z" fill="#DD168D"/>
                        </svg>
                        <div>
                          <p class="text-darker font-semibold text-base">Health Insurance</p>
                          <p class="mt-2 text-current text-sm">Insure yourself </p>
                        </div>
                      </router-link>
                    </li>
                    <li>
                      <router-link to="/products/vehicle" class="flex items-start gap-4">
                        <svg width="50" height="50" viewBox="0 0 50 50" fill="none" xmlns="http://www.w3.org/2000/svg">
                          <circle opacity="0.1" cx="24.9685" cy="24.9685" r="24.9685" fill="#763FA2"/>
                          <path d="M35.3401 23.0479H34.3029L31.6354 17.046C31.5145 16.7745 31.3176 16.5438 31.0684 16.3819C30.8192 16.22 30.5284 16.1337 30.2313 16.1335H18.9377C18.6405 16.1337 18.3497 16.22 18.1006 16.382C17.8514 16.5439 17.6544 16.7746 17.5336 17.046L14.8661 23.0479H13.8288C13.6251 23.0479 13.4296 23.1288 13.2856 23.2729C13.1415 23.417 13.0605 23.6124 13.0605 23.8162C13.0605 24.0199 13.1415 24.2153 13.2856 24.3594C13.4296 24.5035 13.6251 24.5844 13.8288 24.5844H14.5971V32.267C14.5975 32.6744 14.7596 33.065 15.0476 33.353C15.3357 33.6411 15.7262 33.8031 16.1336 33.8036H18.4384C18.8457 33.8031 19.2363 33.6411 19.5244 33.353C19.8124 33.065 19.9744 32.6744 19.9749 32.267V30.7305H29.194V32.267C29.1945 32.6744 29.3565 33.065 29.6446 33.353C29.9327 33.6411 30.3232 33.8031 30.7306 33.8036H33.0354C33.4427 33.8031 33.8333 33.6411 34.1213 33.353C34.4094 33.065 34.5714 32.6744 34.5719 32.267V24.5844H35.3401C35.5439 24.5844 35.7393 24.5035 35.8834 24.3594C36.0275 24.2153 36.1084 24.0199 36.1084 23.8162C36.1084 23.6124 36.0275 23.417 35.8834 23.2729C35.7393 23.1288 35.5439 23.0479 35.3401 23.0479ZM19.9749 27.6575H18.4384C18.2346 27.6575 18.0392 27.5765 17.8951 27.4325C17.7511 27.2884 17.6701 27.093 17.6701 26.8892C17.6701 26.6855 17.7511 26.49 17.8951 26.346C18.0392 26.2019 18.2346 26.121 18.4384 26.121H19.9749C20.1787 26.121 20.3741 26.2019 20.5181 26.346C20.6622 26.49 20.7432 26.6855 20.7432 26.8892C20.7432 27.093 20.6622 27.2884 20.5181 27.4325C20.3741 27.5765 20.1787 27.6575 19.9749 27.6575ZM29.194 27.6575C28.9903 27.6575 28.7949 27.5765 28.6508 27.4325C28.5067 27.2884 28.4258 27.093 28.4258 26.8892C28.4258 26.6855 28.5067 26.49 28.6508 26.346C28.7949 26.2019 28.9903 26.121 29.194 26.121H30.7306C30.9343 26.121 31.1297 26.2019 31.2738 26.346C31.4179 26.49 31.4988 26.6855 31.4988 26.8892C31.4988 27.093 31.4179 27.2884 31.2738 27.4325C31.1297 27.5765 30.9343 27.6575 30.7306 27.6575H29.194Z" fill="#763FA2"/>
                        </svg>
                        <div>
                          <p class="text-darker font-semibold text-base">Vehicle Insurance</p>
                          <p class="mt-2 text-current text-sm">Insure your item</p>
                        </div>
                      </router-link>
                    </li>
                    <li class="relative">
                      <div class="flex items-start gap-4 opacity-50">
                        <svg width="50" height="50" viewBox="0 0 50 50" fill="none" xmlns="http://www.w3.org/2000/svg">
                          <circle opacity="0.1" cx="24.9685" cy="24.9685" r="24.9685" fill="#164EDD"/>
                          <path d="M32.2669 16.1335H16.9017C16.2907 16.1342 15.7048 16.3773 15.2728 16.8094C14.8407 17.2415 14.5976 17.8273 14.5969 18.4383V29.194C14.5976 29.805 14.8407 30.3909 15.2728 30.823C15.7048 31.255 16.2907 31.4981 16.9017 31.4988H23.8161V33.0353H21.5113C21.3075 33.0353 21.1121 33.1162 20.968 33.2603C20.824 33.4044 20.743 33.5998 20.743 33.8036C20.743 34.0073 20.824 34.2027 20.968 34.3468C21.1121 34.4909 21.3075 34.5718 21.5113 34.5718H27.6574C27.8611 34.5718 28.0565 34.4909 28.2006 34.3468C28.3447 34.2027 28.4256 34.0073 28.4256 33.8036C28.4256 33.5998 28.3447 33.4044 28.2006 33.2603C28.0565 33.1162 27.8611 33.0353 27.6574 33.0353H25.3526V31.4988H32.2669C32.878 31.4981 33.4638 31.255 33.8959 30.823C34.328 30.3909 34.571 29.805 34.5717 29.194V18.4383C34.571 17.8273 34.328 17.2415 33.8959 16.8094C33.4638 16.3773 32.878 16.1342 32.2669 16.1335ZM32.2669 29.9623H16.9017C16.698 29.962 16.5028 29.881 16.3587 29.737C16.2147 29.593 16.1337 29.3977 16.1334 29.194V27.6575H33.0352V29.194C33.035 29.3977 32.954 29.593 32.8099 29.737C32.6659 29.881 32.4706 29.962 32.2669 29.9623Z" fill="#164EDD"/>
                        </svg>
                        <div>
                          <p class="text-darker font-semibold text-base">Gadget Insurance</p>
                          <p class="mt-2 text-current text-sm">Insure your item</p>
                        </div>
                      </div>
                      <span class="border bg-white rounded px-3 py-2 hidden absolute top-0 right-0">coming soon</span>
                    </li>

                    <li class="relative">
                      <div class="flex items-start gap-4 opacity-50">
                        <svg  width="50" height="50" viewBox="0 0 50 50" fill="none"  xmlns="http://www.w3.org/2000/svg">
                          <circle opacity="0.1" cx="24.9685" cy="24.9685" r="24.9685" fill="#DDB216"/>
                          <path d="M32.2669 16.1335H16.9017C16.2907 16.1342 15.7048 16.3773 15.2728 16.8094C14.8407 17.2415 14.5976 17.8273 14.5969 18.4383V29.194C14.5976 29.805 14.8407 30.3909 15.2728 30.823C15.7048 31.255 16.2907 31.4981 16.9017 31.4988H23.8161V33.0353H21.5113C21.3075 33.0353 21.1121 33.1162 20.968 33.2603C20.824 33.4044 20.743 33.5998 20.743 33.8036C20.743 34.0073 20.824 34.2027 20.968 34.3468C21.1121 34.4909 21.3075 34.5718 21.5113 34.5718H27.6574C27.8611 34.5718 28.0565 34.4909 28.2006 34.3468C28.3447 34.2027 28.4256 34.0073 28.4256 33.8036C28.4256 33.5998 28.3447 33.4044 28.2006 33.2603C28.0565 33.1162 27.8611 33.0353 27.6574 33.0353H25.3526V31.4988H32.2669C32.878 31.4981 33.4638 31.255 33.8959 30.823C34.328 30.3909 34.571 29.805 34.5717 29.194V18.4383C34.571 17.8273 34.328 17.2415 33.8959 16.8094C33.4638 16.3773 32.878 16.1342 32.2669 16.1335ZM32.2669 29.9623H16.9017C16.698 29.962 16.5028 29.881 16.3587 29.737C16.2147 29.593 16.1337 29.3977 16.1334 29.194V27.6575H33.0352V29.194C33.035 29.3977 32.954 29.593 32.8099 29.737C32.6659 29.881 32.4706 29.962 32.2669 29.9623Z" fill="#DDB216"/>
                        </svg>
                        <div>
                          <p class="text-darker font-semibold text-base">Travel Insurance</p>
                          <p class="mt-2 text-current text-sm">Insure your journey</p>
                        </div>
                      </div>
                      <span class="border bg-white rounded px-3 py-2 hidden absolute top-0 right-0">coming soon</span>
                    </li>
                  </ul>
                </div>
              </div>
            </transition>
          </li>
          <li>
            <router-link to="/impact" class="text-sm text-current hover:text-army pb-3">Impact</router-link>
          </li>
          <li>
            <router-link to="/faq" class="text-sm text-current hover:text-army pb-3">FAQ</router-link>
          </li>
          <li>
            <router-link to="/careers" class="text-sm text-current hover:text-army pb-3">Careers</router-link>
          </li>
          <li>
            <router-link to="/login" class="text-sm text-current hover:text-army pb-3">Sign In</router-link>
          </li>
          <li>
            <router-link to="/signup" class="text-white bg-army py-3 text-sm px-4 rounded-md">Create an account</router-link>
          </li>
        </ul>
      </nav>
    </div>
</template>

<script>
export default {
 data(){
    return {
      showProduct: false
    }
  }
}
</script>

<style scoped>
.product{
  top: 10px;
  left: -100px;
  z-index: 1000;
  min-width: 550px
}
.productlist li:nth-child(1) a:hover p{
  color: #219653
}
li:nth-child(2) a:hover p{
  color: #DD168D
}
li:nth-child(3) a:hover p{
  color: #763FA2
}
li:nth-child(4) a:hover p{
  color: #164EDD
}
li:nth-child(4):hover span{
  display: block;
}

li:nth-child(5) a:hover p{
  color: #ddb216
}
li:nth-child(5):hover span{
  display: block;
}

.slide-enter-active{
  animation-name: slide-in;
  animation-duration: .5s;
}
.slide-leave-active{
  /* animation: slide-in .1s reverse; */
  /* transition: opacity .1s ease-out; */
}
@keyframes slide-in {
  0%{
    opacity: 0;
    transform: translateY(-100px);
  }
  100%{
    opacity: 1;
    transform: translateY(0);
  }
}
@media only screen and (min-width: 1024px){
  nav{
    padding-left: 10%;
    padding-right: 10%;
  }
}
</style>