<!-- +page.svelte -->
<script>
    // Your SvelteKit logic here if needed
</script>

<style>
    /* Additional styles if needed */
</style>

<div class="flex flex-col items-center justify-between min-h-screen bg-gray-100 p-4">
    <!-- Top section with the image and logo -->
    <div class="flex flex-col items-center bg-white shadow-lg rounded-lg p-6 w-full max-w-sm">
        <img src="path_to_your_background_image.jpg" alt="City background" class="w-full h-64 object-cover rounded-t-lg">
        
        <div class="flex flex-col items-center bg-gradient-to-r from-pink-500 to-purple-500 rounded-full p-2 -mt-8">
            <img src="path_to_your_logo_image.svg" alt="College Logo" class="w-20 h-20">
        </div>
        
        <h1 class="text-xl font-bold text-gray-900 mt-4">GCOEN</h1>
        <p class="text-sm text-gray-600">Government College of Engineering, Nagpur</p>
        <p class="text-lg font-semibold text-gray-800 mt-4 text-center">Lajwab bas aur description me details dalo</p>
    </div>

    <!-- Bottom navigation bar -->
    <div class="fixed bottom-0 left-0 right-0 bg-white border-t border-gray-200">
        <div class="flex justify-between p-4 max-w-sm mx-auto">
            <button class="flex flex-col items-center">
                <svg class="w-6 h-6 text-gray-700" fill="currentColor" viewBox="0 0 20 20">
                    <path d="M10 20v-6h4v6h5v-8h3L12 3 2 12h3v8z"></path>
                </svg>
                <span class="text-xs text-gray-700">Home</span>
            </button>
            <button class="flex flex-col items-center">
                <svg class="w-6 h-6 text-gray-700" fill="currentColor" viewBox="0 0 20 20">
                    <path d="M17 8h-1V6a5 5 0 00-10 0v2H5a2 2 0 000 4h12a2 2 0 100-4zM7 6a3 3 0 016 0v2H7V6zM4 10v2a4 4 0 108 0v-2H4z"></path>
                </svg>
                <span class="text-xs text-gray-700">Notifications</span>
            </button>
            <button class="flex flex-col items-center">
                <svg class="w-6 h-6 text-gray-700" fill="currentColor" viewBox="0 0 20 20">
                    <path d="M12 2a1 1 0 00-1 1v2H9V3a1 1 0 00-2 0v2H6a1 1 0 00-.707.293l-3 3A1 1 0 002 9v5a1 1 0 001 1h1v2a1 1 0 002 0v-2h8v2a1 1 0 002 0v-2h1a1 1 0 001-1V9a1 1 0 00-.293-.707l-3-3A1 1 0 0014 5h-1V3a1 1 0 00-1-1zM4.414 9l2-2H13.586l2 2H4.414zM5 14v-3h10v3H5z"></path>
                </svg>
                <span class="text-xs text-gray-700">Messages</span>
            </button>
            <button class="flex flex-col items-center">
                <svg class="w-6 h-6 text-gray-700" fill="currentColor" viewBox="0 0 20 20">
                    <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm-1-11a1 1 0 112 0v4a1 1 0 01-2 0V7zm0 6a1 1 0 112 0 1 1 0 01-2 0z" clip-rule="evenodd"></path>
                </svg>
                <span class="text-xs text-gray-700">Info</span>
            </button>
            <button class="flex flex-col items-center">
                <svg class="w-6 h-6 text-gray-700" fill="currentColor" viewBox="0 0 20 20">
                    <path d="M4 3a2 2 0 00-2 2v10a2 2 0 002 2h12a2 2 0 002-2V5a2 2 0 00-2-2H4zM9 8v8H4V8h5zm7 0v8h-5V8h5zm-7-5v3H4V3h5zm7 0v3h-5V3h5z"></path>
                </svg>
                <span class="text-xs text-gray-700">Profile</span>
            </button>
        </div>
    </div>
</div>
