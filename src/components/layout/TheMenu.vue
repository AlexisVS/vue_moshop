<template>
  <nav class="bg-gray-900 flex justify-around py-3 items-center">
    <router-link to="/">
      <span
        class="text-gray-300 transition duration-500 uppercase font-bold cursor-pointer hover:text-white"
      >Home</span>
    </router-link>
    <router-link to="/shop">
      <span
        class="text-gray-300 transition duration-500 uppercase font-bold cursor-pointer hover:text-white"
      >Shop</span>
    </router-link>
    <div class="flex items-center space-x-6">
      <button
        class="bg-blue-500 text-white shadow-sm py-1 px-6 font-bold rounded-md uppercase hover:bg-blue-600"
      @click="displayedModalLogin = !displayedModalLogin"
      >Login</button>
      <button
        class="bg-white text-blue-500 hover:text-blue-400 shadow-sm py-1 px-6 font-bold rounded-md uppercase hover:bg-gray-200"
      @click="displayedModalRegister = !displayedModalRegister"
      >Register</button>
    </div>
    <Login v-show="displayedModalLogin" @toggleLoginOverlay="displayedModalLogin = !displayedModalLogin"/>
    <Register v-show="displayedModalRegister" @toggleRegisterOverlay="displayedModalRegister = !displayedModalRegister"/>
  </nav>
</template>

<script>
import Login from './menu/Login.vue';
import Register from './menu/Register.vue';
export default {
  components: {
    Login,
    Register,
  },
  data () {
    return {
      displayedModalLogin: false,
      displayedModalRegister: false,
    }
  }
}
</script>

<style>
</style>