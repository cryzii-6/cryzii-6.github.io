<script>
    let userName = 'Ynnyannah'; 
</script>

<style>
    :global(body) {
        font-family: 'Poppins', sans-serif;
    }

    .navbar {
        position: absolute;
        top: 20px; /* Adjust based on your design */
        left: 50%;
        transform: translateX(-50%);
        background: rgba(255, 255, 255, 0.8);
        padding: 10px 20px;
        border-radius: 25px;
        box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
        z-index: 20; /* Ensure it's above other elements */
    }

    .navbar a {
        margin: 0 15px;
        text-decoration: none;
        color: #4a90e2;
        font-weight: bold;
    }

    .navbar a:hover {
        text-decoration: underline;
    }
</style>

<main class="relative flex items-center justify-center h-screen bg-gradient-to-r from-blue-600 to-teal-500 text-white overflow-hidden">
    <div class="absolute inset-0">
        <div class="bg-circle bg-yellow-400 opacity-20 w-64 h-64 absolute top-10 left-10 animate-pulse"></div>
        <div class="bg-circle bg-teal-300 opacity-20 w-96 h-96 absolute bottom-20 right-20 animate-pulse"></div>
        <div class="bg-triangle bg-blue-300 opacity-20 w-48 h-48 absolute top-32 right-40"></div>
        <div class="bg-triangle bg-purple-400 opacity-20 w-80 h-80 absolute bottom-28 left-56"></div>
        <div class="bg-star bg-pink-400 opacity-30 w-32 h-32 absolute top-5 right-5 animate-spin-slow"></div>
        <div class="bg-star bg-orange-400 opacity-30 w-48 h-48 absolute bottom-10 left-10 animate-spin-slow"></div>
    </div>

    <nav class="navbar">
        <a href="portfolio">Portfolio</a>
        <a href="about">About</a>
        <a href="contact">Contact</a>
    </nav>
  
    <div class="relative text-center space-y-6 p-8 bg-white bg-opacity-10 backdrop-blur-lg rounded-xl shadow-2xl max-w-sm hover:shadow-3xl transition-all duration-500 ease-in-out transform hover:scale-105 z-10">
        <h1 class="text-5xl font-bold leading-tight">Hey There, {userName}!</h1>
        <p class="text-xl text-white/80">Welcome to the platform.</p>
    </div>
</main>
