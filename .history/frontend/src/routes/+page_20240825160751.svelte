<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Signup Page</title>
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
        <h2 class="text-3xl font-extrabold text-center text-gray-800 mb-8">Join Our Community</h2>

        <div class="flex justify-center mb-6 space-x-4">
            <button id="student-btn" class="text-blue-600 font-semibold px-4 py-2 hover:text-blue-700 transition duration-300 border-b-4 border-blue-600">Student</button>
            <button id="alumni-btn" class="text-green-600 font-semibold px-4 py-2 hover:text-green-700 transition duration-300 border-b-4 border-green-600">Alumni</button>
            <button id="college-btn" class="text-purple-600 font-semibold px-4 py-2 hover:text-purple-700 transition duration-300 border-b-4 border-purple-600">College</button>
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
            <p class="text-center text-gray-500 mt-4">Already have an account? <a href="#" id="student-login" class="text-blue-600 hover:underline">Login</a></p>
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
            <p class="text-center text-gray-500 mt-4">Already have an account? <a href="#" id="alumni-login" class="text-green-600 hover:underline">Login</a></p>
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
            <p class="text-center text-gray-500 mt-4">Already have an account? <a href="#" id="college-login" class="text-purple-600 hover:underline">Login</a></p>
        `;

        function redirectToLogin(type) {
            // Placeholder for redirect logic, replace with actual navigation code
            alert(`Redirecting to ${type} login page...`);
            // window.location.href = `/${type}-login.html`; // Example of how to redirect
        }

        studentBtn.addEventListener('click', () => {
            form.innerHTML = studentForm;
            document.getElementById('student-login').addEventListener('click', () => redirectToLogin('student'));
        });

        alumniBtn.addEventListener('click', () => {
            form.innerHTML = alumniForm;
            document.getElementById('alumni-login').addEventListener('click', () => redirectToLogin('alumni'));
        });

        collegeBtn.addEventListener('click', () => {
            form.innerHTML = collegeForm;
            document.getElementById('college-login').addEventListener('click', () => redirectToLogin('college'));
        });

        // Load the default form (student form)
        form.innerHTML = studentForm;
        document.getElementById('student-login').addEventListener('click', () => redirectToLogin('student'));
    </script>
</body>

</html>
