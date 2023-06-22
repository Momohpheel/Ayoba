<template>
  <section class="pt-10 pb-6 px-4 lg:pt-16 lg:px-16">
      <div class="flex justify-between items-center">
          <h2 class="text-darker font-bold text-2xl lg:text-center lg:flex-grow">Explore our Products</h2>
          <div class="flex gap-2 items-center lg:hidden">
              
          </div>
      </div>
      <ul class="mt-10 gap-8 w-full lg:justify-center lg:mx-auto lg:gap-4">
        <li class="flex-shrink-0 min-w-[200px] max-w-[25%] pb-3">
            <router-link to="/products/health" class="block w-full p-4 bg-fuschia rounded-lg">
                  <p class="text-white text-sm">Health & Accident Insurance</p>
                  <div class="flex justify-end mt-6">
                     
                  </div>
              </router-link>
          </li>
          <li class="flex-shrink-0 min-w-[200px] max-w-[25%] pb-3">
            <router-link to="/products/vehicle" class="block w-full p-4 bg-violet rounded-lg">
                  <p class="text-white text-sm">Vehicle & Motorcycle Insurance</p>
                  <div class="flex justify-end mt-6">
                     
                  </div>
              </router-link>
          </li>  
        <li class="min-w-[200px] max-w-[15%] pb-3">
            <router-link to="/products/homecontent" class="w-full block p-4 bg-army rounded-lg">
                  <p class="text-white text-sm">Home Content Insurance</p>
                  <div class="flex justify-end mt-6">
                      
                  </div>
              </router-link>
          </li>
         
          <li class="flex-shrink-0 min-w-[200px] max-w-[25%] pb-3">
            <div class="w-full p-4 bg-navy rounded-lg">
                  <p class="text-white text-sm">Gadgets & POS Insurance</p>
                  <div class="flex justify-end mt-6">
                      
                  </div>
              </div>
          </li>
          <li class="flex-shrink-0 min-w-[200px] max-w-[25%] pb-3">
            <div class="w-full p-4 bg-yellow-400 rounded-lg">
                  <p class="text-white text-sm">Travel Insurance</p>
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
          </li>
          <li class="flex-shrink-0 min-w-[200px] max-w-[25%]">
            <div class="w-full p-4 bg-gray-900 rounded-lg">
                  <p class="text-white text-sm">Pet Insurance</p>
                  <div class="flex justify-end mt-8">
                      
                      <div class="bg-white px-4 rounded-full opacity-30">
                        
                      </div>
      
                  </div>
              </div>
          </li>
      </ul>
  </section>
</template>

<script>
export default {

}
</script>

<style scoped>
ul::-webkit-scrollbar{
    height: 0;
    display: none
}
@media only screen and (min-width: 1024px){
    h2{
        font-size: 40px
    }
    ul{
        max-width: 1500px
    }
}
</style>