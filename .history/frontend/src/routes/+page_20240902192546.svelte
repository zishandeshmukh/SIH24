<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.6.0/css/all.min.css">
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@3.2.4/dist/tailwind.min.css" rel="stylesheet">
</head>
<body class="flex">
    <!-- <img id="imag" src="public/assets/img_2.jpeg" alt="alum_img" class="w-2/3 h-screen object-cover"> -->
    <img id="imag" src="images.png" alt="alum_img" class="w-2/3 h-screen object-cover">


    <div class="flex-1 flex items-center justify-center p-4">
        <div class="bg-white rounded-lg shadow-lg p-6 max-w-md w-full animate-fadeIn">
            <p id="login" class="text-center text-xl font-semibold">Log in to Alumni Connect</p>
            <form action="" class="mt-4">
                <input type="text" id="username" name="username" placeholder="Student Id"  required class="w-full p-2.5 mb-4 border-none rounded-lg text-lg bg-gray-100 outline-none">
                <input type="password" id="password" name="password" placeholder="Password" required class="w-full p-2.5 mb-4 border-none rounded-lg text-lg bg-gray-100 outline-none">
                <p class="text-gray-600 text-center mb-4">
                    <a href="forgot_password.html" class="text-blue-600">Forgot Password?</a>
                </p>
                <input id="submit" type="submit" value="Login" class="w-full p-2.5 mb-4 border-none rounded-lg text-lg bg-red-600 text-white cursor-pointer">
                <p id="suggest" class="text-gray-600 text-center text-lg mb-4">Or login with</p>
                <button class="w-full p-2.5 mb-4 border-none rounded-lg text-lg bg-gray-200 flex items-center justify-center">
                    <i class="fa-brands fa-google mr-2"></i> Google
                </button>
                <button class="w-full p-2.5 mb-4 border-none rounded-lg text-lg bg-gray-200 flex items-center justify-center">
                    <i class="fa-brands fa-github mr-2"></i> Github
                </button>
                <button class="w-full p-2.5 mb-4 border-none rounded-lg text-lg bg-gray-200 flex items-center justify-center">
                    <i class="fa-brands fa-linkedin mr-2"></i> LinkedIn
                </button>
                <p id="suggest" class="text-gray-600 text-center text-lg">Don't have an account? 
                    <a href="login.svelte" id="signup" class="text-red-600">Sign up now</a>
                </p>
            </form>
        </div>
    </div>
</body>
</html>