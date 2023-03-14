<template>
  <div class="mt-5">
   <div class="relative">

    
      <ul class="mt-10 gap-8 w-full lg:justify-center lg:mx-auto lg:gap-4">
         
          <li class="flex-shrink-0 min-w-[200px] max-w-[25%]">
            <div class="flex">
            <router-link to="/app/dashboard/buyhealth/1" class="block w-full p-4 mx-1 bg-fuschia rounded-lg">
                  <p class="text-white text-sm">Health & Accident Insurance</p>
                  <div class="flex justify-end mt-6">
                     
                  </div>
              </router-link>

              <router-link to="/app/dashboard/managehealth" class="block w-full p-4 bg-fuschia rounded-lg">
                  <p class="text-white text-sm">Manage Your Health & Accident Policy</p>
                  <div class="flex justify-end mt-6">
                     
                  </div>
              </router-link>
            </div>
          </li>
          <li class="flex-shrink-0 min-w-[200px] max-w-[25%]">
            <div class="flex">
            <router-link to="/app/dashboard/buyvehicle/1" class="block w-full p-4 mx-1 bg-violet rounded-lg">
                  <p class="text-white text-sm">Vehicle & Motorcycle Insurance</p>
                  <div class="flex justify-end mt-6">
                     
                  </div>
              </router-link>

              <router-link to="/app/dashboard/managevehicle" class="block w-full p-4 bg-violet rounded-lg">
                  <p class="text-white text-sm">Manage Your Vehicle & Motorcycle Insurance</p>
                  <div class="flex justify-end mt-6">
                     
                  </div>
              </router-link>
            </div>
          </li>
          <li class="min-w-[200px] max-w-[15%]">
            <div class="flex">
            <router-link to="/products/homecontent" class="w-full block p-4 mx-1 bg-army rounded-lg">
                  <p class="text-white text-sm">Home Content Insurance</p>
                  <div class="flex justify-end mt-6">
                      
                  </div>
              </router-link>

              <router-link to="/app/dashboard/managehome" class="w-full block p-4 bg-army rounded-lg">
                  <p class="text-white text-sm">Manage Your Home Content Insurance</p>
                  <div class="flex justify-end mt-6">
                      
                  </div>
              </router-link>

            </div>
          </li>
          <li class="flex-shrink-0 min-w-[200px] max-w-[25%]">
            <div class="flex">
            <div class="w-full p-4 mx-1 bg-navy rounded-lg">
                  <p class="text-white text-sm">Gadgets & POS Insurance</p>
                  <div class="flex justify-end mt-6">
                      
                  </div>
              </div>

              <div class="w-full p-4 bg-navy rounded-lg">
                  <p class="text-white text-sm">Manage Your Gadgets & POS Insurance</p>
                  <div class="flex justify-end mt-6">
                      
                  </div>
              </div>
            </div>
          </li>
          <li class="flex-shrink-0 min-w-[200px] max-w-[25%]">

            <div class="flex">
            <div class="w-full p-4 mx-1 bg-yellow-400 rounded-lg">
                  <p class="text-white text-sm">Travel & Travel Insurance</p>
                  <div class="flex justify-end mt-8">
                      <!-- <button>
                           <svg width="72" height="72" viewBox="0 0 72 72" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <circle opacity="0.1" cx="36" cy="36" r="36" fill="white"/>
                                <g opacity="0.5">
                                    <path d="M30.1708 16.9999V90.9999C30.1708 21.1479 30.1379 21.294 30.0746 21.4277C30.0114 21.5615 29.9192 21.6795 29.8047 21.7733C29.6903 21.8671 29.5565 21.9343 29.413 21.9702C29.2694 22.006 29.1197 22.0096 28.9746 21.9805L20.1708 20.2197V23.5899L21.8547 25.2979C22.0392 25.485 22.1426 25.7372 22.1426 25.9999V28.9999C22.1426 29.1634 22.1025 29.3243 22.026 29.4686C21.9494 29.613 21.8386 29.7364 21.7032 29.828C21.5679 29.9196 21.4122 29.9767 21.2497 29.9942C21.0873 30.0117 20.923 29.9891 20.7712 29.9284L16.1426 28.077L11.5139 29.9284C11.3622 29.9891 11.1979 30.0117 11.0354 29.9942C10.8729 29.9767 10.7172 29.9196 10.5819 29.828C10.4466 29.7364 10.3358 29.613 10.2592 29.4686C10.1826 29.3243 10.1426 29.1634 10.1426 28.9999V25.9999C10.1426 25.7347 10.2479 25.4804 10.4354 25.2928L12.1426 23.5857V20.2197L3.33875 21.9805C3.19366 22.0096 3.04395 22.006 2.90039 21.9702C2.75684 21.9343 2.62303 21.8671 2.50861 21.7733C2.39418 21.6795 2.302 21.5615 2.2387 21.4277C2.17541 21.294 2.14258 21.1479 2.14258 20.9999V16.9999C2.14257 16.8142 2.19428 16.6322 2.2919 16.4742C2.38953 16.3163 2.52922 16.1886 2.69531 16.1055L12.144 11.3812L12.1566 5.99762C12.1569 4.93675 12.5786 3.91946 13.329 3.16953C14.0794 2.4196 15.0969 1.99847 16.1578 1.99878C17.2186 1.99909 18.2359 2.42081 18.9859 3.17117C19.7358 3.92154 20.1569 4.93907 20.1566 5.99994L20.1693 11.3812L29.618 16.1055C29.7841 16.1886 29.9238 16.3163 30.0215 16.4742C30.1191 16.6322 30.1708 16.8142 30.1708 16.9999Z" fill="white"></path>
                                </g>
                            </svg>
                       
                      </button> -->
                      <div class="bg-white px-4 rounded-full opacity-30">
                        
                      </div>
      
                  </div>
              </div>

              <div class="w-full p-4 bg-yellow-400 rounded-lg">
                  <p class="text-white text-sm">Manage Your Travel Insurance</p>
                  <div class="flex justify-end mt-8">
                      <!-- <button>
                           <svg width="72" height="72" viewBox="0 0 72 72" fill="none" xmlns="http://www.w3.org/2000/svg">
                                <circle opacity="0.1" cx="36" cy="36" r="36" fill="white"/>
                                <g opacity="0.5">
                                    <path d="M30.1708 16.9999V90.9999C30.1708 21.1479 30.1379 21.294 30.0746 21.4277C30.0114 21.5615 29.9192 21.6795 29.8047 21.7733C29.6903 21.8671 29.5565 21.9343 29.413 21.9702C29.2694 22.006 29.1197 22.0096 28.9746 21.9805L20.1708 20.2197V23.5899L21.8547 25.2979C22.0392 25.485 22.1426 25.7372 22.1426 25.9999V28.9999C22.1426 29.1634 22.1025 29.3243 22.026 29.4686C21.9494 29.613 21.8386 29.7364 21.7032 29.828C21.5679 29.9196 21.4122 29.9767 21.2497 29.9942C21.0873 30.0117 20.923 29.9891 20.7712 29.9284L16.1426 28.077L11.5139 29.9284C11.3622 29.9891 11.1979 30.0117 11.0354 29.9942C10.8729 29.9767 10.7172 29.9196 10.5819 29.828C10.4466 29.7364 10.3358 29.613 10.2592 29.4686C10.1826 29.3243 10.1426 29.1634 10.1426 28.9999V25.9999C10.1426 25.7347 10.2479 25.4804 10.4354 25.2928L12.1426 23.5857V20.2197L3.33875 21.9805C3.19366 22.0096 3.04395 22.006 2.90039 21.9702C2.75684 21.9343 2.62303 21.8671 2.50861 21.7733C2.39418 21.6795 2.302 21.5615 2.2387 21.4277C2.17541 21.294 2.14258 21.1479 2.14258 20.9999V16.9999C2.14257 16.8142 2.19428 16.6322 2.2919 16.4742C2.38953 16.3163 2.52922 16.1886 2.69531 16.1055L12.144 11.3812L12.1566 5.99762C12.1569 4.93675 12.5786 3.91946 13.329 3.16953C14.0794 2.4196 15.0969 1.99847 16.1578 1.99878C17.2186 1.99909 18.2359 2.42081 18.9859 3.17117C19.7358 3.92154 20.1569 4.93907 20.1566 5.99994L20.1693 11.3812L29.618 16.1055C29.7841 16.1886 29.9238 16.3163 30.0215 16.4742C30.1191 16.6322 30.1708 16.8142 30.1708 16.9999Z" fill="white"></path>
                                </g>
                            </svg>
                       
                      </button> -->
                      <div class="bg-white px-4 rounded-full opacity-30">
                        
                      </div>
      
                  </div>
              </div>
            </div>
          </li>
      </ul>
    <!-- <ul class="horizontalmenu flex justify-between gap-8 lg:gap-5" ref="horizontalmenu">
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
            
          <router-link to="/app/dashboard/buytravel/1" class="block mt-4 bg-green-500 font-bold text-white rounded px-4 py-2 ">Buy</router-link>
          </div>
        </div>
      </li>
        
    </ul> -->
    
  </div>
 
    
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