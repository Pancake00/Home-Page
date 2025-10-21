<template>
  <div class="min-h-screen flex items-center justify-center bg-gradient-to-br from-blue-100 to-blue-300">
    <div class="bg-white shadow-2xl rounded-2xl p-10 w-full max-w-md">
      <h1 class="text-3xl font-bold text-center text-blue-700 mb-8">Welcome Back</h1>
      <form @submit.prevent="login" class="space-y-6">
        <div>
          <label class="block text-sm font-semibold text-gray-600 mb-2">Username</label>
          <input
            v-model="email"
            type="text"
            placeholder="Enter your username"
            class="w-full border border-gray-300 rounded-lg px-4 py-2 focus:ring-2 focus:ring-blue-500 focus:outline-none"
          />
        </div>
        <div>
          <label class="block text-sm font-semibold text-gray-600 mb-2">Password</label>
          <input
            v-model="password"
            type="password"
            placeholder="Enter your password"
            class="w-full border border-gray-300 rounded-lg px-4 py-2 focus:ring-2 focus:ring-blue-500 focus:outline-none"
          />
        </div>
        <button
          type="submit"
          class="w-full bg-blue-600 text-white font-semibold py-2 rounded-lg hover:bg-blue-700 transition duration-200"
        >
          Login
        </button>
      </form>
      <p class="text-center text-gray-600 mt-6">
        Don’t have an account?
        <router-link to="/register" class="text-blue-600 hover:underline font-medium">Sign Up</router-link>
      </p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      email: "",
      password: ""
    };
  },
  methods: {
    login() {
      const correctUsername = "emilys";
      const correctPassword = "emilyspass";

      if (this.email === correctUsername && this.password === correctPassword) {
        // ✅ Route to the Dashboard page
        this.$router.push("/dashboard");
      } else {
        alert("Invalid username or password. Please try again.");
      }
    }
  }
};
</script>
