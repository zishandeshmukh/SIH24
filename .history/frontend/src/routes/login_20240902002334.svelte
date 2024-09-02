<script>
    // Import any required modules here
</script>

<style>
    body {
        background-image: url('https://source.unsplash.com/1600x900/?education,college');
        background-size: cover;
        background-position: center;
        background-repeat: no-repeat;
    }
</style>

<div class="bg-white shadow-2xl rounded-lg p-8 max-w-md w-full bg-opacity-90">
    <h2 class="text-2xl font-bold text-center text-gray-800 mb-8">Login</h2>
    
    <form class="space-y-4">
        <div>
            <label class="block text-gray-700">Email</label>
            <input type="email" class="w-full border-gray-300 rounded-lg shadow-sm focus:ring-blue-400" placeholder="Enter your Email">
        </div>
        <div>
            <label class="block text-gray-700">Password</label>
            <input type="password" class="w-full border-gray-300 rounded-lg shadow-sm focus:ring-blue-400" placeholder="Enter Password">
        </div>
        <button type="submit" class="w-full bg-blue-600 text-white rounded-lg py-2 hover:bg-blue-700 transition duration-300">Login</button>
        <p class="text-center text-gray-500 mt-4">Don't have an account? <a href="/" class="text-blue-600 hover:underline">Sign Up</a></p>
    </form>
</div>
