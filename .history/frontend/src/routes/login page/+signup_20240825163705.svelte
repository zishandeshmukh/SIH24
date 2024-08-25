<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login Page</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        body {
            background-image: url('https://source.unsplash.com/1600x900/?education,college,learning');
            background-size: cover;
            background-position: center;
            background-repeat: no-repeat;
        }

        .backdrop {
            background: rgba(255, 255, 255, 0.8);
            backdrop-filter: blur(10px);
        }
    </style>
</head>

<body class="bg-gray-900 min-h-screen flex flex-col justify-center items-center">

    <div class="backdrop shadow-2xl rounded-lg p-8 max-w-md w-full">
        <h2 class="text-3xl font-extrabold text-center text-gray-800 mb-8">Login</h2>

        <form class="space-y-6">
            <div>
                <label class="block text-gray-700">Student ID</label>
                <input type="text" class="w-full border-gray-300 rounded-lg shadow-sm focus:ring focus:ring-blue-400 focus:ring-opacity-50 transition duration-300" placeholder="Enter your Student ID">
            </div>
            <div>
                <label class="block text-gray-700">Password</label>
                <input type="password" class="w-full border-gray-300 rounded-lg shadow-sm focus:ring focus:ring-blue-400 focus:ring-opacity-50 transition duration-300" placeholder="Enter your Password">
            </div>
            <button class="w-full bg-blue-600 text-white rounded-lg py-2 hover:bg-blue-700 transition duration-300">Login</button>
            <p class="text-center text-gray-500 mt-4">Don't have an account? <a href="signup.html" class="text-blue-600 hover:underline">Sign Up</a></p>
        </form>
    </div>

</body>

</html>
