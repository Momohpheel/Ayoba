<template>
  <div class="lg:hidden pt-6">
      <div class="bg-white px-3 flex justify-between items-center">
        <router-link to="/"><img src="@/assets/logo.svg" alt="" style="width: 80px"></router-link>
        <button @click="$store.commit('toggleHomeCollapse')" type="button">
          <svg width="26" height="22" viewBox="0 0 26 22" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M1 10.9999H25M1 1.3999H25M1 20.5999H25" stroke="#0F2217" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
          </svg>
        </button>
      </div>
      <transition name="slidedown">
        <div v-if="$store.state.homeCollapse" class="fixed w-full left-0 py-4 pb-6 bg-white mobilemenu h-full">
          <div class="px-4 flex justify-between items-center">
            <router-link to="/"><img src="@/assets/logo.svg" alt="" style="width: 80px"></router-link>
            <button @click="$store.commit('toggleHomeCollapse')" type="button">
              <svg width="25" height="26" viewBox="0 0 25 26" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M1 25L24 1.5" stroke="#0F2217" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                <path d="M24 25L1 1.5" stroke="#0F2217" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
              </svg>
            </button>
          </div>
          <ul class="mt-14 px-3">
            
            
            
            <li class="mt-6 text-center font-medium">
              <router-link to="/login" class="text-army text-sm py-3 px-10 bg-white border border-solid border-army rounded-md">Sign in</router-link>
            </li>
            <li class="mt-10 text-center font-medium">
              <router-link to="/signup" class="text-white text-sm py-3 px-2 bg-army rounded-md">Create an Account</router-link>
            </li>
          </ul>
        </div>
      </transition>
    </div>
</template>

<script>
export default {
    data(){
        return {
            showProducts : false
        }
    }

}
</script>

<style>
li:nth-child(4):hover span{
  display: block;
}
li:nth-child(5):hover span{
  display: block;
}
.mobilemenu{
  top: 0;
  width: 100%;
  left: 0;
  box-shadow: 0px 9px 45px #00000090;
  z-index: 1002
}
.slidedown-enter-active{
  animation-name: slide-down;
  animation-duration: .5s;
}
.slidedown-leave-active{
  animation: slide-down .5s reverse;
  /* transition: opacity .1s ease-out; */
}
.fade-enter-active{
  animation-name: fadeIn;
  animation-duration: .5s;
}
.fade-leave-active{
  animation: fadeIn .5s reverse;
}
@keyframes slide-down {
  0%{
    transform: translateY(-300px);
  }
  100%{
    transform: translateY(0);
  }
}
@keyframes fadeIn {
  0%{
    opacity: 0;
  }
  100%{
    opacity: 1;
  }
}
</style>