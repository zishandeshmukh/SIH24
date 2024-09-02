<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@3.0.0/dist/tailwind.min.css" rel="stylesheet">
</head>
<body class="bg-[#0d1b2a]">
    <!-- navbar -->
    <div class="flex items-center justify-between h-[7vh] px-4 bg-[#010100]">
        <div class="flex items-center">
            <img id="logo_img" class="w-28 rounded-lg" src="alum_new_logo.png" alt="Logo">
        </div>
        <ul class="flex items-center ml-auto mr-6 space-x-4">
            <li><a class="text-[#EFECEF] py-4 hover:text-gray-300 transition-transform transform hover:scale-105" href="index.html">Home</a></li>
            <li><a class="text-[#EFECEF] py-4 hover:text-gray-300 transition-transform transform hover:scale-105" href="job.html">Job Portal</a></li>
            <li><a class="text-[#EFECEF] py-4 hover:text-gray-300 transition-transform transform hover:scale-105" href="donation.html">Donation</a></li>
            <li><a class="text-[#EFECEF] py-4 hover:text-gray-300 transition-transform transform hover:scale-105" href="announcement.html">Announcement</a></li>
        </ul>
    </div>
    
    <section id="prof" class="absolute right-4 top-4 flex items-center justify-center w-8 h-8 rounded-full bg-gray-600">
        <i id="profile" class="text-white text-xl cursor-pointer fa-solid fa-user"></i>
    </section>

    <button id="menu_button" class="hidden text-white opacity-50 ml-2 mt-5 bg-none border-none cursor-pointer text-xl">
        <i class="fa-solid fa-bars"></i>
    </button>

    <div id="sidebar" class="fixed left-0 top-0 h-full w-52 bg-[#373737] z-50 p-4 shadow-md overflow-y-auto hidden">
        <button id="close_button" class="absolute top-2 right-2 bg-none border-none cursor-pointer text-white text-xl">
            <i class="fa-solid fa-xmark"></i>
        </button>
        <ul class="space-y-4">
            <li><a class="text-white py-2 px-4 block bg-[#373737] hover:bg-[#555]" href="index.html">Home</a></li>
            <li><a class="text-white py-2 px-4 block bg-[#373737] hover:bg-[#555]" href="job.html">Job Portal</a></li>
            <li><a class="text-white py-2 px-4 block bg-[#373737] hover:bg-[#555]" href="donation.html">Donation</a></li>
            <li><a class="text-white py-2 px-4 block bg-[#373737] hover:bg-[#555]" href="announcement.html">Announcement</a></li>
        </ul>
    </div>

    <div class="flex flex-col w-3/5 mx-auto mt-16 bg-[#212121] text-white p-4">
        <div id="back_img_section" class="h-1/4 w-full bg-[#2c2a2a]">
            <img id="back_img" class="w-full h-full object-cover" src="background.webp" alt="">
        </div>
        <div id="profile_img_section" class="w-28 h-28 bg-clip-content rounded-full bg-white mx-auto mt-[-2rem] flex items-center justify-center">
            <img id="image" class="w-full h-full rounded-full" src="profile.jpg" alt="">
        </div>
        <div id="name_sec" class="flex flex-col mt-4 ml-6">
            <p id="name" class="text-2xl">Vinay Titarmare</p>
            <p id="college" class="mt-2">Student at Government College of Engineering</p>
            <p id="address" class="mt-1 opacity-80">Maharashtra, India <a id="contact" class="text-blue-400 pl-2" href="#">Contact Me</a></p>
        </div>
        <div id="post_connection" class="flex justify-around my-4">
            <div id="post" class="text-center">
                <p id="no" class="text-xl">45</p>
                <p>Posts</p>
            </div>
            <div id="follower" class="text-center">
                <p id="no" class="text-xl">48</p>
                <p>Follower</p>
            </div>
            <div id="connection" class="text-center">
                <p id="no" class="text-xl">264</p>
                <p>Connections</p>
            </div>
        </div>
        <div id="profile_modifications" class="flex justify-around my-4">
            <button id="edit" class="bg-aqua border-3 border-[#0d1b2a] rounded-lg py-2 px-4">Edit Profile</button>
            <button id="share" class="bg-aqua border-3 border-[#0d1b2a] rounded-lg py-2 px-4">Share Profile</button>
        </div>
        <hr class="my-4">
        <div id="profile_posts" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4 p-4 bg-[#212121] text-[#333] mb-12">
            <div class="post bg-[#484748] h-[40vh]"></div>
            <div class="post bg-[#484748] h-[40vh]"></div>
            <div class="post bg-[#484748] h-[40vh]"></div>
            <div class="post bg-[#484748] h-[40vh]"></div>
        </div>
    </div>

    <script src="script.js"></script>
</body>
</html>