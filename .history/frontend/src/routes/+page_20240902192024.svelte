<script>
    import { goto } from '$app/navigation';

    let formType = 'student';

    function showForm(type) {
        formType = type;
    }

    function redirectToLogin() {
        goto('/login');
    }
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
    <h2 class="text-2xl font-bold text-center text-gray-800 mb-8">Join Our Community</h2>
    
    <div class="flex justify-center mb-6">
        <button on:click={() => showForm('student')} class="text-blue-600 font-semibold mx-2 hover:text-blue-700 transition duration-300">Student</button>
        <button on:click={() => showForm('alumni')} class="text-green-600 font-semibold mx-2 hover:text-green-700 transition duration-300">Alumni</button>
        <button on:click={() => showForm('college')} class="text-purple-600 font-semibold mx-2 hover:text-purple-700 transition duration-300">College</button>
    </div>

    {#if formType === 'student'}
        <form class="space-y-4">
            <div>
                <label class="block text-gray-700">Student ID</label>
                <input type="text" class="w-full border-gray-300 rounded-lg shadow-sm focus:ring-blue-400" placeholder="Enter your Student ID">
            </div>
            <div>
                <label class="block text-gray-700">Generate Password</label>
                <input type="password" class="w-full border-gray-300 rounded-lg shadow-sm focus:ring-blue-400" placeholder="Enter Password">
            </div>
            <div>
                <label class="block text-gray-700">Continue with Email</label>
                <input type="email" class="w-full border-gray-300 rounded-lg shadow-sm focus:ring-blue-400" placeholder="Enter your Email">
            </div>
            <div>
                <input type="text" class="w-full border-gray-300 rounded-lg shadow-sm focus:ring-blue-400" placeholder="Enter your Phone Number">
            </div>
            <button type="submit" class="w-full bg-blue-600 text-white rounded-lg py-2 hover:bg-blue-700 transition duration-300">Sign Up</button>
            <p class="text-center text-gray-500 mt-4">Already have an account? <button on:click={redirectToLogin} class="text-blue-600 hover:underline">Login</button></p>
        </form>
    {/if}
    {#if formType === 'alumni'}
        <!-- Alumni Form Content -->
    {/if}
    {#if formType === 'college'}
        <!-- College Form Content -->
    {/if}
</div>
