<template>
  <div
    class="flex items-center justify-center w-full h-screen bg-gray-100 bg-opacity-25 max-w-screen z-20 absolute top-0 left-0"
    @click="$emit('toggleRegisterOverlay', false)"
  >
    <div class="w-full max-w-3xl overflow-hidden rounded-lg shadow-lg sm:flex z-50" @click.stop>
      <div
        class="w-full text-white bg-gray-700 bg-center bg-cover sm:w-2/5"
        style="background-image: url('https://images.unsplash.com/photo-1504985954001-5737b2af529e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2879&q=80')"
      ></div>
      <div class="w-full bg-white sm:w-3/5">
        <div class="p-8">
          <h1 class="text-3xl font-black">SIGN UP</h1>
          <p class="mt-2 mb-5 text-base leading-tight text-gray-600">
            Create an account to join our awesome
            community
          </p>
          <form>
            <label for="email" class="text-xs text-gray-500">email</label>
            <input
              id="email"
              class="block rounded-md w-full pb-1 m-auto mb-6 text-gray-700 bg-transparent border-b border-gray-500"
              type="text"
              placeholder
            />
            <label id="passowrd" class="text-xs text-gray-500">Password</label>
            <input
              id="password"
              class="block rounded-md w-full pb-1 m-auto mb-6 bg-transparent border-b border-gray-500 text-grey-700"
              type="password"
              placeholder
            />
            <label id="firstName" class="text-xs text-gray-500">first name</label>
            <input
              id="firstName"
              class="block rounded-md w-full pb-1 m-auto mb-6 bg-transparent border-b border-gray-500 text-grey-700"
              type="text"
              placeholder
            />
            <label id="lastName" class="text-xs text-gray-500">Last name</label>
            <input
              id="lastName"
              class="block rounded-md w-full pb-1 m-auto mb-6 bg-transparent border-b border-gray-500 text-grey-700"
              type="text"
              placeholder
            />
            <label id="picture" class="text-xs text-gray-500">Picture</label>
            <input
              id="picture"
              class="block rounded-md w-full pb-1 m-auto mb-6 bg-transparent border-b border-gray-500 text-grey-700"
              type="file"
              placeholder
            />
            <input
              class="w-full rounded-md pt-3 pb-3 text-white bg-indigo-500 shadow-lg cursor-pointer hover:bg-indigo-400"
              type="submit"
              value="Create account"
            />
          </form>
          <div class="mt-4 text-center">
            <p class="text-sm text-gray-600">
              Already have an account?
              <a
                href="#"
                class="font-bold text-indigo-500 no-underline hover:text-indigo-400"
              >Sign in</a>
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data () {

  }
}
</script>

<style>
</style>