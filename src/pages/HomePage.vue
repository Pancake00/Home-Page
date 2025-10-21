<template>
  <div class="min-h-screen w-full flex flex-col bg-gradient-to-br from-blue-100 via-blue-300 to-blue-500">
    <!-- Navigation Bar -->
    <header class="bg-white/20 backdrop-blur-md py-4 shadow-md">
      <div class="max-w-7xl mx-auto flex justify-between items-center px-6">
        <h1 class="text-2xl font-bold text-blue-900">Vue Login Lab</h1>
        <nav class="space-x-4">
          <router-link to="/login" class="text-blue-900 hover:underline font-semibold">Login</router-link>
          <router-link to="/register" class="text-blue-900 hover:underline font-semibold">Sign Up</router-link>
        </nav>
      </div>
    </header>

    <!-- Hero Section -->
    <main class="flex flex-1 items-center justify-center px-6">
      <div class="text-center bg-white/80 backdrop-blur-md p-16 rounded-3xl shadow-2xl max-w-3xl w-full">
        <h1 class="text-5xl font-extrabold text-blue-800 mb-6">Welcome to Our App</h1>
        <p class="text-gray-700 text-lg mb-10 leading-relaxed">
          Start your journey today 
        </p>
        <div class="flex justify-center space-x-6">
          <router-link
            to="/login"
            class="px-8 py-3 bg-blue-700 text-white font-semibold text-lg rounded-xl shadow hover:bg-blue-800 transition duration-200"
          >
            Login
          </router-link>
          <router-link
            to="/register"
            class="px-8 py-3 bg-white border-2 border-blue-700 text-blue-700 font-semibold text-lg rounded-xl hover:bg-blue-100 transition duration-200"
          >
            Sign Up
          </router-link>
        </div>
      </div>
    </main>

    <!-- Footer -->
    <footer class="bg-white/20 backdrop-blur-md py-4 text-center text-blue-900 text-sm font-medium">
      © 2025 Vue Login Lab. All rights reserved.
    </footer>
  </div>
</template>

<script>
export default {};
</script>
