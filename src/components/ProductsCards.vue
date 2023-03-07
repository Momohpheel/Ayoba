<template>
  <div class="mt-12">
   <div class="relative">
    <ul class="horizontalmenu flex justify-between gap-8 lg:gap-5" ref="horizontalmenu">
      <button @click="scrollLeft" class="rightbutt  md:flex lg:flex absolute shadow-lg bg-green-200 opacity-30 hover:opacity-100 rounded-full items-center justify-center" style="width: 70px; height: 70px">
        
            <svg width="24" height="24" viewBox="0 0 24 24"  fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M15.7131 12L9.70209 5.99001L8.28809 7.40401L12.8881 12.004L8.28809 16.597L9.70209 18.011L15.7131 12Z" fill="#2E3A59"></path>
            </svg>
        
      </button>
      <li class="rounded tile">
        <div class="bg-white px-6 py-3 lg:py-6 lg:px-8 text-center rounded">
          <p class="font-bold text-lg">Health Insurance</p>
          <img src="../assets/images/menu/Image 9.png" alt="" class="mt-4 mx-auto w-3/5 lg:w-full img" >
          <p class="mb-6 mt-4">{{healthtext | slicer}} <span class="block text-blue-500 underline cursor-pointer" @click="showModal(1)">read more</span></p>
          <router-link to="/app/dashboard/managehealth" class=" block mt-10 text-green-500 font-bold border border-solid border-gray-200 rounded px-4 py-2">Manage Policy</router-link>
          <router-link to="/app/dashboard/buyhealth/1" class="block mt-4 bg-green-500 font-bold text-white rounded px-4 py-2 ">Buy</router-link>
        </div>
      </li>
      <li class="rounded tile">
        <div class="bg-white px-6 py-3 lg:py-6 lg:px-8 text-center rounded">
          <p class="font-bold text-lg">Vehicle Insurance</p>
          <img src="../assets/images/menu/Group 65.png" alt="" class="mt-4 mx-auto w-3/5 lg:w-full img" >
          <p class="mb-6 mt-4">{{vehicletext | slicer}} <span class="block text-blue-500 underline cursor-pointer" @click="showModal(2)">read more</span></p>
          <div v-if="!$store.state.user.has_address" class="relative" @mouseover="showInfo = true" @mouseleave="showInfo = false" @click="showInfo = !showInfo">
            <p class=" block mt-10 text-green-500 opacity-30 font-bold border border-solid border-gray-200 rounded px-4 py-2">Manage Policy</p>
            <p class="block mt-4 bg-green-500 opacity-30 font-bold text-white rounded px-4 py-2 ">Buy </p>
            <div v-if="showInfo" class="bg-white text-sm rounded absolute py-4 px-4 left-0 top-6 showInfo shadow-md" style="width: 200px">
              <p>Add your home address to buy vehicle insurance</p>
              <p class="text-blue-500 cursor-pointer" @click="addAddress">Add now</p>
            </div>
          </div>
          <div v-else>
            <router-link to="/app/dashboard/managevehicle" class="block mt-10 text-green-500 font-bold border border-solid border-gray-200 rounded px-4 py-2">Manage Policy</router-link>
            <router-link to="/app/dashboard/buyvehicle/1" class="block mt-4 bg-green-500 font-bold text-white rounded px-4 py-2 ">Buy</router-link>
          </div>
        </div>
      </li>
      <li class="rounded tile">
        <div class="bg-white px-6 py-3 lg:py-6 lg:px-8 text-center rounded">
          <p class="font-bold text-lg">Home content</p>
          <img src="../assets/images/menu/Image 10.png" alt="" class="mt-4 mx-auto w-3/5 lg:w-full img" >
          <p class="mb-6 mt-4">{{hometext | slicer}} <span class="block text-blue-500 underline cursor-pointer" @click="showModal(3)">read more</span></p>
          <router-link to="/app/dashboard/managehome" class=" block mt-10 text-green-500 font-bold border border-solid border-gray-200 rounded px-4 py-2">Manage Policy</router-link>
          <router-link to="/app/dashboard/buyhome/1" class="block mt-4 bg-green-500 font-bold text-white rounded px-4 py-2 ">Buy</router-link>
        </div>
      </li>
      <li class="rounded tile">
        <div class="bg-white px-6 py-3 lg:py-6 lg:px-8 text-center rounded">
          <p class="font-bold text-lg">Gadget Cover</p>
          <img src="../assets/images/menu/Image 11.png" alt="" class="mt-4 mx-auto w-3/5 lg:w-full img" >
          <p class="mb-6 mt-4">{{gadgettext | slicer}} <span class="block text-blue-500 underline cursor-pointer" @click="showModal(4)">read more</span></p>
          <div class="relative" >
            <p class=" block mt-10 text-green-500 opacity-30 font-bold border border-solid border-gray-200 rounded px-4 py-2">Manage Policy</p>
            <p class="block mt-4 bg-green-500 opacity-30 font-bold text-white rounded px-4 py-2 ">Coming Soon</p>
          </div>
        </div>
      </li>
      <li class="rounded tile">
        <div class="bg-white px-9 py-3 lg:py-6 lg:px-8 text-center rounded">
          <p class="font-bold text-lg">Travel Cover</p>
          <img src="../assets/images/menu/travel.png" alt="" class="mt-4 mx-auto w-3/5 lg:w-full img" >
          <p class="mb-9 mt-4">{{gadgettext | slicer}} <span class="block text-blue-500 underline cursor-pointer">read more</span></p>
          <div class="relative" >
            <br/>
            <br/>
            <!-- <router-link to="/app/dashboard/managetravel" class=" block mt-13 mb-3 text-green-500 font-bold   px-4 py-2"></router-link> -->
          <router-link to="/app/dashboard/buytravel/1" class="block mt-4 bg-green-500 font-bold text-white rounded px-4 py-2 ">Buy</router-link>
          </div>
        </div>
      </li>
        
    </ul>
    <button @click="scrollRight" class="leftbutt md:flex lg:flex absolute shadow-lg bg-green-300 opacity-30 hover:opacity-100 bg-transparent rounded-full items-center justify-center" style="width: 70px; height: 70px">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M15.7131 12L9.70209 5.99001L8.28809 7.40401L12.8881 12.004L8.28809 16.597L9.70209 18.011L15.7131 12Z" fill="#2E3A59"></path>
                </svg>
        </button>
  </div>
 
    <p class="mt-6 lg:mt-8 text-sm lg:text-center">It’s important to note that you can purchase more than one policy and you can also add a dependent to any or multiple of these policies</p>
    <AboutHealth v-if="activeModal == 1" v-on:close="closeActiveModal"/>
    <AboutVehicle v-if="activeModal == 2" v-on:close="closeActiveModal"/>
    <AboutHome v-if="activeModal == 3" v-on:close="closeActiveModal"/>
    <AboutGadget v-if="activeModal == 4" v-on:close="closeActiveModal"/>
  
  </div>
</template>

<script>
import AboutHealth from "@/components/Health/AboutModal"
import AboutHome from "@/components/Home/AboutModal"
import AboutVehicle from "@/components/Vehicle/AboutModal"
import AboutGadget from "@/components/Gadget/AboutModal"
import {mapState} from "vuex"
export default {
  components:{
    AboutHealth, AboutHome, AboutGadget, AboutVehicle
  },
  data(){
    return {
      showInfo: false,
      showList1: false,
      activeModal: 0,
      vehicletext: "For insurance on vehicles ranging from full repairs, third-party repair, outright replacement",
      healthtext: "For insurance on healthcare ranging from Surgeries, Therapy, Dentals amongst others",
      gadgettext: "For insurance on gadgets ranging from Repairs, Refurbishing,  amongst others",
      hometext: "Home Insurance protects you financially in the event that your home and property are damaged as a result of a burglary or fire outbreak. It is designed essentially for those living in rented apartments to cover their contents only against loss as a result of burglary, fire & special peril.Home Insurance protects you financially in the event that your home and property are damaged as a result of a burglary or fire outbreak. It is designed essentially for those living in rented apartments to cover their contents only against loss as a result of burglary, fire & special peril.",
    }
  },
  computed:{
    ...mapState({
      user : state => state.user
    })
  },
  methods:{
    scrollRight(){
            this.$refs.horizontalmenu.scrollLeft += 250
        },
        scrollLeft(){
            this.$refs.horizontalmenu.scrollLeft -= 250
        },
    showModal(num){
      this.activeModal = num;
      this.$store.commit('setActiveModal', num)
    },
    closeActiveModal(){
      this.activeModal = 0;
      this.$store.commit('setActiveModal', 0)
    },
    // to keep track of where the user is coming from in orderto redirect them back
    addAddress(){
      this.$store.commit('addAddress', true)
      this.$router.push("/app/dashboard/settings")
    }
  },
  filters:{
    slicer(val){
      return val.slice(0, 40) + '...'
    }
  },
  
}
</script>


<style scoped>

.horizontalmenu::-webkit-scrollbar{
    height: 0
}
.horizontalmenu{
    scroll-behavior: smooth;
}
.showInfo{
    z-index: 100000
  }
ul{
  flex-wrap: nowrap;
  overflow-x: auto;
}

.tile{
  flex: 0 0 auto;
  margin-left: 20px;
  margin-right: 20px;
  max-width: 250px;
  box-shadow: 0 20px 33px #00000029;
  /* z-index: 100 */
}
  ul li{
    margin-bottom: 20px
  }
ul::-webkit-scrollbar-track{
  box-shadow: inset 0 0 6px rgba(0,0,0,0.3);
  border-radius: 10px;
  background-color: #F5F5F5;
}

ul::-webkit-scrollbar
{
  margin-top: 20px;
  height: 2px;
  background-color: #F5F5F5;
}

ul::-webkit-scrollbar-thumb
{
  border-radius: 10px;
  box-shadow: inset 0 0 6px rgba(0,0,0,.3);
  background-color: #14801B;
}
.tile img{
  height: 100px;
}
@media only screen and (min-width: 1280px){
  .tile img{
    width: 120px;
    height: 100px
  }
  ul{
    display: flex;
    overflow-x: hidden;
    justify-content: space-between;
    box-shadow: 0 20px 33px #00000029;
  }
  .tile{
    flex: 0 0 25%;
    margin-left: 0;
    margin-right: 0;
    display: inline-block;
    /* width: 20%; */
    /* margin: 3% */
    
  }
  .tile img{
    width: 100px;
    height: 100px
    /* height: 162px */
  }
 
}

@media only screen and (min-width: 1024px){
  .leftbutt{
        top: 50%;
        transform: translateY(-50%);
        right: -40px
    }

    .rightbutt{
        top: 50%;
        transform: translateY(-50%);
        left: -40px
    }
}

@media only screen and (min-width: 350px){
  .leftbutt{
        top: 50%;
        transform: translateY(-50%);
        right: -40px
    }

    .rightbutt{
        top: 50%;
        transform: translateY(-50%);
        left: -40px
    }
}

@media only screen and (min-width: 480px){
  .leftbutt{
        top: 50%;
        transform: translateY(-50%);
        right: -40px
    }

    .rightbutt{
        top: 50%;
        transform: translateY(-50%);
        left: -40px
    }
}

@media only screen and (min-width: 768px){
  .leftbutt{
        top: 50%;
        transform: translateY(-50%);
        right: -40px
    }

    .rightbutt{
        top: 50%;
        transform: translateY(-50%);
        left: -40px
    }
}
</style>