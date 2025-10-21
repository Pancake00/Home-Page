
<template>
  <div class="min-h-screen bg-gray-100 flex flex-col">
    <header class="bg-blue-700 text-white py-4 shadow-md">
      <div class="container mx-auto flex justify-between items-center px-6">
        <h1 class="text-2xl font-bold">Dashboard</h1>
        <button @click="logout" class="bg-white text-blue-700 px-4 py-1 rounded-lg font-semibold hover:bg-gray-200 transition">Logout</button>
      </div>
    </header>

    <main class="flex-grow container mx-auto px-6 py-8">
      <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
        <div class="bg-white rounded-2xl shadow-md p-6 hover:shadow-xl transition">
          <h2 class="text-xl font-bold text-blue-700 mb-2">Welcome</h2>
          <p class="text-gray-600">You are now logged in. Explore your data and insights below.</p>
        </div>

        <div class="bg-white rounded-2xl shadow-md p-6 hover:shadow-xl transition">
          <h2 class="text-xl font-bold text-blue-700 mb-2">Analytics</h2>
          <p class="text-gray-600">Placeholder for analytics content or widgets.</p>
        </div>

        <div class="bg-white rounded-2xl shadow-md p-6 hover:shadow-xl transition">
          <h2 class="text-xl font-bold text-blue-700 mb-2">Settings</h2>
          <p class="text-gray-600">Manage your preferences and profile details here.</p>
        </div>
      </div>
    </main>

    <footer class="bg-blue-700 text-white text-center py-3 text-sm mt-auto">
      © 2025 Your App. All rights reserved.
    </footer>
  </div>
</template>

<script>
export default {
  methods: {
    logout() {
      // existing logout logic remains
      console.log("Logged out");
    }
  }
};
</script>
