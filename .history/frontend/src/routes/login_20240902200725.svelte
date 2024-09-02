<!-- +page.svelte -->
<script>
  // Your SvelteKit logic can go here if needed
</script>

<div class="flex flex-col items-center justify-between min-h-screen bg-gray-100">
  <!-- Top section with the image and logo -->
  <div class="w-full max-w-xs bg-white shadow-lg rounded-lg overflow-hidden">
    <!-- Background Image -->
    <div class="relative">
      <img src="path_to_your_background_image.jpg" alt="Cityscape Background" class="w-full h-64 object-cover">
      <!-- Logo with Gradient Background -->
      <div class="absolute -bottom-10 left-1/2 transform -translate-x-1/2 bg-gradient-to-r from-pink-500 to-purple-500 rounded-full p-2">
        <img src="path_to_your_logo_image.svg" alt="College Logo" class="w-20 h-20">
      </div>
    </div>
    <!-- Content Section -->
    <div class="mt-12 p-4 text-center">
      <h1 class="text-xl font-bold text-gray-900">GCOEN</h1>
      <p class="text-sm text-gray-600">Government College of Engineering, Nagpur</p>
      <p class="mt-4 text-lg font-semibold text-gray-800">Lajwab bas aur description me details dalo</p>
    </div>
  </div>

  <!-- Bottom Navigation Bar -->
  <div class="fixed bottom-0 left-0 right-0 bg-white shadow-md">
    <div class="flex justify-around py-2">
      <button class="flex flex-col items-center text-gray-700">
        <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6" fill="currentColor" viewBox="0 0 20 20">
          <path d="M10 20v-6h4v6h5v-8h3L12 3 2 12h3v8z"></path>
        </svg>
        <span class="text-xs">Home</span>
      </button>
      <button class="flex flex-col items-center text-gray-700">
        <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6" fill="currentColor" viewBox="0 0 20 20">
          <path d="M10 2a1 1 0 00-1 1v2H7V3a1 1 0 00-2 0v2H4a1 1 0 00-.707.293l-3 3A1 1 0 000 9v7a1 1 0 001 1h2a1 1 0 001 1v-3h10v3a1 1 0 001 1h2a1 1 0 001-1V9a1 1 0 00-.293-.707l-3-3A1 1 0 0016 5h-1V3a1 1 0 00-2 0v2h-2V3a1 1 0 00-1-1zM4.414 9l2-2h7.172l2 2H4.414zM2 14v-4h16v4H2z"></path>
        </svg>
        <span class="text-xs">Messages</span>
      </button>
      <button class="flex flex-col items-center text-gray-700">
        <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6" fill="currentColor" viewBox="0 0 20 20">
          <path d="M2 11a1 1 0 011-1h14a1 1 0 011 1v5a1 1 0 01-1 1H3a1 1 0 01-1-1v-5zM18 7V5a4 4 0 00-4-4H6a4 4 0 00-4 4v2h16zM6 7V5a2 2 0 014 0v2H6z"></path>
        </svg>
        <span class="text-xs">Profile</span>
      </button>
      <button class="flex flex-col items-center text-gray-700">
        <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6" fill="currentColor" viewBox="0 0 20 20">
          <path d="M8 9V6a4 4 0 118 0v3h-1V6a3 3 0 00-6 0v3H8zM7 8V6a5 5 0 0110 0v2a3 3 0 110 6H3a3 3 0 110-6V6a5 5 0 0110 0v2h-1V6a4 4 0 00-8 0v2h-2v4h16V8H7z"></path>
        </svg>
        <span class="text-xs">Settings</span>
      </button>
      <button class="flex flex-col items-center text-gray-700">
        <svg xmlns="http://www.w3.org/2000/svg" class="w-6 h-6" fill="currentColor" viewBox="0 0 20 20">
          <path d="M4 3a2 2 0 00-2 2v10a2 2 0 002 2h12a2 2 0 002-2V5a2 2 0 00-2-2H4zM9 8v8H4V8h5zm7 0v8h-5V8h5zm-7-5v3H4V3h5zm7 0v3h-5V3h5z"></path>
        </svg>
        <span class="text-xs">Info</span>
      </button>
    </div>
  </div>
</div>
