<template>
  <form @submit.prevent="validateForm" class="w-full">
        <div class="w-full">
            <p class="mt-6 text-sm cursor-pointer" @click="$emit('hideNext')"><font-awesome-icon class="mr-1" icon="arrow-left"/> Back</p>
            <div class="lg:mt-6">
            <label class="text-army font-bold">Password</label>
            <div class="mt-2 bg-white w-full rounded relative">
                <input type="password" v-model="user.password" ref="password" class="w-full py-2 px-3 rounded outline-none border border-gray-200 focus:outline-none focus:ring-1 focus:ring-army focus:border-transparent focus:border-0" required>
                <font-awesome-icon icon="eye" v-if="showEye" class="absolute eye text-gray-500" @click="showPassword"/>
                <font-awesome-icon icon="eye-slash" v-else class="absolute eye text-gray-500" @click="hidePassword"/>
            </div>
            <p v-if="error.password" class="text-red-500 text-sm mt-2">Your password should contain at least 8 characters (at least one uppercase, one lowercase, one special character and one number)</p>
            <!-- <p class="text-xs mt-4 font-semibold">Password must contain an uppercase letter, a number, a special character and 8 characters long</p> -->
            </div>
            <div class="mt-4 lg:mt-6">
            <label class="text-army font-bold">Confirm Password</label>
            <input type="password" v-model="confirm" ref="confirm" class="mt-2 w-full py-2 px-3 rounded outline-none border border-gray-200 focus:outline-none focus:ring-1 focus:ring-army focus:border-transparent focus:border-0" required>
            <p v-if="error.confirm" class="text-red-500 text-sm mt-2">Your passwords don't match</p>
            </div>
            <button class="mt-10 outline-none py-2 rounded w-full text-white focus:outline-none" style="background-color: #00A859">Sign up</button>
        </div>
        <router-link to="/login" class="inline-block mt-6 text-center rounded focus:outline-none bg-gray-100 text-charcoal py-2 w-full text-white">Log in if you already have an account</router-link>
    </form>
</template>

<script>
export default {
    data(){
     return {
        showEye: true,
        user:{
            password: ""
        },
        confirm: "",
        error:{
            password: false,
            confirm: false,
        }
     }   
    },
    computed:{
        password(){
            return this.user.password
        }
    },
    watch:{
        password(){
            if(/^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)(?=.*[@$!%*#?&^])[A-Za-z\d@$!%*#?&^]{8,}$/.test(this.user.password)){
                this.error.password = false
            }else{
                this.error.password = true
            }
        },
        confirm(){
            if(this.confirm !== this.user.password){
                this.error.confirm = true
                
            }else{
                this.error.confirm = false
            }
        }
    },
    methods:{
        showPassword(){
            this.$refs.password.type = 'text'
            this.$refs.confirm.type = 'text'
            this.showEye = false
        },
        hidePassword(){
            this.$refs.password.type = 'password'
            this.$refs.confirm.type = 'password'
            this.showEye = true
        },
        validateForm(){
            if(Object.values(this.error).includes(true)){
                return
            }else{
                // console.log(this.user)
             this.$emit('updateUser', this.user)  
            }
        }
    }
}
</script>

<style scoped>
.greent{
  color: #2CB675
}
.blue-bg{
  background-color: #E2F5EC;
}
.eye{
  top: 0;
  bottom: 0;
  margin: auto 0;
  right: 5px;
  cursor: pointer;
}
</style>