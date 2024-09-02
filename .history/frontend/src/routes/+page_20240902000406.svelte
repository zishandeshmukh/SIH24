<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Signup Page</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        body {
            background-image: url('https://source.unsplash.com/1600x900/?education,college');
            background-size: cover;
            background-position: center;
            background-repeat: no-repeat;
        }
    </style>
</head>
<body class="bg-opacity-80 bg-gray-900 min-h-screen flex flex-col justify-center items-center">

    <div class="bg-white shadow-2xl rounded-lg p-8 max-w-md w-full bg-opacity-90">
        <h2 class="text-2xl font-bold text-center text-gray-800 mb-8">Join Our Community</h2>
        
        <div class="flex justify-center mb-6">
            <button id="student-btn" class="text-blue-600 font-semibold mx-2 hover:text-blue-700 transition duration-300">Student</button>
            <button id="alumni-btn" class="text-green-600 font-semibold mx-2 hover:text-green-700 transition duration-300">Alumni</button>
            <button id="college-btn" class="text-purple-600 font-semibold mx-2 hover:text-purple-700 transition duration-300">College</button>
        </div>

        <form id="signup-form" class="space-y-4">
            <!-- Form content will be inserted here dynamically -->
        </form>
    </div>

    <script>
        const form = document.getElementById('signup-form');
        const studentBtn = document.getElementById('student-btn');
        const alumniBtn = document.getElementById('alumni-btn');
        const collegeBtn = document.getElementById('college-btn');

        const inputStyles = "w-full border-gray-300 rounded-lg shadow-sm focus:ring focus:ring-opacity-50 transition duration-300";
        <script>
    import { goto } from '$app/navigation';
</script>

<a href="/next-page" class="text-blue-500 underline">Go to Next Page via Link</a>

<button on:click={() => goto('/next-page')} class="bg-blue-500 text-white py-2 px-4 rounded">
    Go to Next Page via Button
</button>

        const studentForm = `
            <div>
                <label class="block text-gray-700">Student ID</label>
                <input type="text" class="${inputStyles} focus:ring-blue-400" placeholder="Enter your Student ID">
            </div>
            <div>
                <label class="block text-gray-700">Generate Password</label>
                <input type="password" class="${inputStyles} focus:ring-blue-400" placeholder="Enter Password">
            </div>
            <div>
                <label class="block text-gray-700">Continue with Email</label>
                <input type="email" class="${inputStyles} focus:ring-blue-400" placeholder="Enter your Email">
            </div>
            <div>
                <input type="text" class="${inputStyles} focus:ring-blue-400" placeholder="Enter your Phone Number">
            </div>
            <button class="w-full bg-blue-600 text-white rounded-lg py-2 hover:bg-blue-700 transition duration-300">Sign Up</button>
            <p class="text-center text-gray-500 mt-4">Already have an account? <a href="#" class="text-blue-600 hover:underline">Login</a></p>
        `;

        const alumniForm = `
            <div>
                <label class="block text-gray-700">Student ID</label>
                <input type="text" class="${inputStyles} focus:ring-green-400" placeholder="Enter your Student ID">
            </div>
            <div>
                <label class="block text-gray-700">Generate Password</label>
                <input type="password" class="${inputStyles} focus:ring-green-400" placeholder="Enter Password">
            </div>
            <div>
                <label class="block text-gray-700">Continue with Email</label>
                <input type="email" class="${inputStyles} focus:ring-green-400" placeholder="Enter your Email">
            </div>
            <div>
                <input type="text" class="${inputStyles} focus:ring-green-400" placeholder="Enter your Phone Number">
            </div>
            <button class="w-full bg-green-600 text-white rounded-lg py-2 hover:bg-green-700 transition duration-300">Sign Up</button>
            <p class="text-center text-gray-500 mt-4">Already have an account? <a href="#" class="text-green-600 hover:underline">Login</a></p>
        `;

        const collegeForm = `
            <div>
                <label class="block text-gray-700">College Name</label>
                <input type="text" class="${inputStyles} focus:ring-purple-400" placeholder="Enter College Name">
            </div>
            <div>
                <label class="block text-gray-700">College ID</label>
                <input type="text" class="${inputStyles} focus:ring-purple-400" placeholder="Enter College ID">
            </div>
            <div>
                <label class="block text-gray-700">Generate Password</label>
                <input type="password" class="${inputStyles} focus:ring-purple-400" placeholder="Enter Password">
            </div>
            <button class="w-full bg-purple-600 text-white rounded-lg py-2 hover:bg-purple-700 transition duration-300">Sign Up</button>
            <p class="text-center text-gray-500 mt-4">Already have an account? <a href="#" class="text-purple-600 hover:underline">Login</a></p>
        `;

        studentBtn.addEventListener('click', () => {
            form.innerHTML = studentForm;
        });

        alumniBtn.addEventListener('click', () => {
            form.innerHTML = alumniForm;
        });

        collegeBtn.addEventListener('click', () => {
            form.innerHTML = collegeForm;
        });

        // Load the default form (student form)
        form.innerHTML = studentForm;
    </script>
</body>
</html>
