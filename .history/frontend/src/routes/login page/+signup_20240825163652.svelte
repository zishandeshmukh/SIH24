<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Signup Page</title>
    <script src="https://cdn.tailwindcss.com"></script>
</head>
<body class="bg-gray-100 min-h-screen flex flex-col justify-center items-center">

    <div class="bg-white shadow-lg rounded-lg p-8 max-w-md w-full">
        <div class="flex justify-center mb-6">
            <button id="student-btn" class="text-blue-500 font-semibold mx-2">Student</button>
            <button id="alumni-btn" class="text-blue-500 font-semibold mx-2">Alumni</button>
            <button id="college-btn" class="text-blue-500 font-semibold mx-2">College</button>
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

        const studentForm = `
            <div>
                <label class="block text-gray-700">Student ID</label>
                <input type="text" class="w-full border-gray-300 rounded-lg shadow-sm focus:ring focus:ring-opacity-50 focus:ring-blue-500" placeholder="Enter your Student ID">
            </div>
            <div>
                <label class="block text-gray-700">Generate Password</label>
                <input type="password" class="w-full border-gray-300 rounded-lg shadow-sm focus:ring focus:ring-opacity-50 focus:ring-blue-500" placeholder="Enter Password">
            </div>
            <div>
                <label class="block text-gray-700">Continue with</label>
                <input type="email" class="w-full border-gray-300 rounded-lg shadow-sm focus:ring focus:ring-opacity-50 focus:ring-blue-500" placeholder="Enter your Email">
            </div>
            <div>
                <input type="text" class="w-full border-gray-300 rounded-lg shadow-sm focus:ring focus:ring-opacity-50 focus:ring-blue-500" placeholder="Enter your Phone Number">
            </div>
            <button class="w-full bg-blue-500 text-white rounded-lg py-2">Sign Up</button>
            <p class="text-center text-gray-500 mt-4">Already have an account? <a href="#" class="text-blue-500">Login</a></p>
        `;

        const alumniForm = `
            <div>
                <label class="block text-gray-700">Student ID</label>
                <input type="text" class="w-full border-gray-300 rounded-lg shadow-sm focus:ring focus:ring-opacity-50 focus:ring-blue-500" placeholder="Enter your Student ID">
            </div>
            <div>
                <label class="block text-gray-700">Generate Password</label>
                <input type="password" class="w-full border-gray-300 rounded-lg shadow-sm focus:ring focus:ring-opacity-50 focus:ring-blue-500" placeholder="Enter Password">
            </div>
            <div>
                <label class="block text-gray-700">Continue with</label>
                <input type="email" class="w-full border-gray-300 rounded-lg shadow-sm focus:ring focus:ring-opacity-50 focus:ring-blue-500" placeholder="Enter your Email">
            </div>
            <div>
                <input type="text" class="w-full border-gray-300 rounded-lg shadow-sm focus:ring focus:ring-opacity-50 focus:ring-blue-500" placeholder="Enter your Phone Number">
            </div>
            <button class="w-full bg-blue-500 text-white rounded-lg py-2">Sign Up</button>
            <p class="text-center text-gray-500 mt-4">Already have an account? <a href="#" class="text-blue-500">Login</a></p>
        `;

        const collegeForm = `
            <div>
                <label class="block text-gray-700">College Name</label>
                <input type="text" class="w-full border-gray-300 rounded-lg shadow-sm focus:ring focus:ring-opacity-50 focus:ring-blue-500" placeholder="Enter College Name">
            </div>
            <div>
                <label class="block text-gray-700">College ID</label>
                <input type="text" class="w-full border-gray-300 rounded-lg shadow-sm focus:ring focus:ring-opacity-50 focus:ring-blue-500" placeholder="Enter College ID">
            </div>
            <div>
                <label class="block text-gray-700">Generate Password</label>
                <input type="password" class="w-full border-gray-300 rounded-lg shadow-sm focus:ring focus:ring-opacity-50 focus:ring-blue-500" placeholder="Enter Password">
            </div>
            <button class="w-full bg-blue-500 text-white rounded-lg py-2">Sign Up</button>
            <p class="text-center text-gray-500 mt-4">Already have an account? <a href="#" class="text-blue-500">Login</a></p>
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
