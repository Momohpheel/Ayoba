<template>
   <div class="l-modal">
      <div class="loading-modal w-full px-4 md:px-0">
        <u-animate-container>
          <u-animate
            name="slideInDown"
            delay="0s"
            duration="0.6s"
            :iteration="1"
            animateClass="animated"
            :begin="true"
            class="loader bg-white md:w-4/5 mx-auto rounded px-4 lg:px-8 lg:pb-6"
            v-on-clickaway="close"
          >
            <div class="pt-6">
              <div class="flex justify-between">
                <div>
                  <img src="@/assets/images/menu/Image 9.png" alt="" class="img">  
                  <p class="text-sm mt-4 cursor-pointer font-bold text-lg">
                    About Health Insurance
                  </p>
                </div>
                <font-awesome-icon icon="times-circle" class="cursor-pointer text-red-500 text-base lg:text-xl" @click="$emit('close')" />
              </div>
              <p class="mt-4">Health insurance helps covers the cost of an insured individual's medical and surgical expenses. There are various plan types, and they vary in terms of what you need.Get a health cover that is designed to suit your specific needs and enjoy access to quality healthcare and superior service delivery An affordable health plan with access to quality healthcare for you & your loved ones. Pay as low as ₦1,500 monthly.</p>
            </div>
          </u-animate>
        </u-animate-container>
      </div>
    </div>
</template>

<script>
import "animate.css"
import { directive as onClickaway } from 'vue-clickaway';
export default {
  data(){
    return {
      existing: ''
    }
  },
  methods:{
    close(){
      this.$emit('close')
    }
  },
  directives: {
    onClickaway: onClickaway,
  }
}
</script>

<style scoped>
.loader{
  position: relative;
  top: 5px;
  padding-bottom: 20px;
  min-height: 80vh
}
.img{
  width: 120px
}
p{
  text-align: justify;
}
@media only screen and (min-width: 1024px){
  .loader{
    width: 600px
  }
}
</style>