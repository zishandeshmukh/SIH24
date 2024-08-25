<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>College Login</title>
    <script src="https://cdn.tailwindcss.com"></script>
</head>

<body class="bg-gray-100 min-h-screen flex flex-col justify-center items-center">

    <div class="bg-white shadow-lg rounded-lg p-8 max-w-md w-full">
        <h2 class="text-2xl font-bold text-center text-gray-800 mb-6">College Login</h2>
        <form class="space-y-4">
            <div>
                <label class="block text-gray-700">College ID</label>
                <input type="text" class="w-full border-gray-300 rounded-lg shadow-sm focus:ring focus:ring-blue-500" placeholder="Enter your College ID">
            </div>
            <div>
                <label class="block text-gray-700">Password</label>
                <input type="password" class="w-full border-gray-300 rounded-lg shadow-sm focus:ring focus:ring-blue-500" placeholder="Enter your Password">
            </div>
            <button class="w-full bg-blue-500 text-white rounded-lg py-2">Login</button>
            <p class="text-center text-gray-500 mt-4">Don't have an account? <a href="signup.html" class="text-blue-500">Sign Up</a></p>
        </form>
    </div>
</body>

</html>
