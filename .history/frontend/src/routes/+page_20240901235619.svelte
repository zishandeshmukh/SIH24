<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/tailwindcss@3.2.4/dist/tailwind.min.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.6.0/css/all.min.css">
</head>
<body class="m-0 p-0 bg-gray-100">
    <div class="w-full max-w-sm p-5 bg-white rounded-lg shadow-lg animate-fade-in mx-auto mt-10">
        <p class="text-xl font-semibold text-center">Log in to Alumni Connect</p>
        <form action="">
            <input type="text" id="username" name="username" placeholder="Student Id" class="w-full py-2 px-4 mb-2 border-none rounded-lg text-lg bg-gray-200 outline-none">
            <input type="password" id="password" name="password" placeholder="Password" class="w-full py-2 px-4 mb-2 border-none rounded-lg text-lg bg-gray-200 outline-none">
            <p class="text-center text-gray-600">
                <a href="forgot_password.html" class="text-blue-500 hover:underline">Forgot Password?</a>
            </p>
            <input id="submit" type="submit" value="Login" class="w-full py-2 px-4 mb-2 border-none rounded-lg text-white bg-orange-600 outline-none text-lg cursor-pointer hover:bg-orange-700">
            <p class="text-center text-gray-600 text-lg">Or login with</p>
            <button class="w-full py-2 px-4 mb-2 border-none rounded-lg bg-gray-200 text-lg flex items-center justify-center">
                <i class="fa-brands fa-google mr-2"></i> Google
            </button>
            <button class="w-full py-2 px-4 mb-2 border-none rounded-lg bg-gray-200 text-lg flex items-center justify-center">
                <i class="fa-brands fa-facebook mr-2"></i> Facebook
            </button>
            <p class="text-center text-gray-600 text-lg">
                Don't have an account? <a href="index.html" class="text-orange-600 hover:underline">Sign up now</a>
            </p>
        </form>
    </div>
</body>
</html>