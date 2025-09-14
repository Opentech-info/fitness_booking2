<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Lipataka | Coming Soon</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">
  <script src="https://cdn.tailwindcss.com"></script>
  <script src="https://unpkg.com/@lottiefiles/lottie-player@latest/dist/lottie-player.js"></script>
  <style>
    body {
      font-family: 'Poppins', sans-serif;
      background: linear-gradient(-45deg, #0f0c29, #302b63, #24243e, #1a1a2e);
      background-size: 400% 400%;
      animation: gradient 12s ease infinite;
    }
    @keyframes gradient {
      0% {background-position: 0% 50%;}
      50% {background-position: 100% 50%;}
      100% {background-position: 0% 50%;}
    }
    .glass {
      background: rgba(255, 255, 255, 0.1);
      backdrop-filter: blur(15px);
      border: 1px solid rgba(255, 255, 255, 0.2);
    }
    .neon-text {
      text-shadow: 0 0 10px #ff00ff, 0 0 20px #ff00ff, 0 0 30px #ff33cc;
    }
    .glow:hover {
      box-shadow: 0 0 15px #00e1ff, 0 0 25px #00e1ff;
      transform: scale(1.1);
    }
  </style>
</head>
<body class="min-h-screen flex flex-col items-center justify-center text-white p-6">

  <!-- Title -->
  <div class="text-center space-y-4">
    <h1 class="text-5xl md:text-7xl font-extrabold neon-text animate-bounce">
      🚀 Lipataka
    </h1>
    <h2 class="text-xl md:text-2xl font-semibold tracking-wide text-white/90">
      Something cool is cooking... Stay tuned!
    </h2>
  </div>

  <!-- Cartoon Animation -->
  <div class="my-10">
    <lottie-player 
      src="https://assets1.lottiefiles.com/packages/lf20_jcikwtux.json"  
      background="transparent"  
      speed="1"  
      style="width: 320px; height: 320px;"  
      loop  
      autoplay>
    </lottie-player>
  </div>

  <!-- Glassmorphism Card -->
  <div class="glass rounded-3xl shadow-2xl p-8 text-center max-w-xl w-full">
    <p class="text-lg leading-relaxed mb-6">
      At <span class="font-bold text-pink-400">Lipataka.com</span>, we’re crafting a powerful experience with 
      modern tech, clean design, and startup vibes 🌟
    </p>

    <!-- Progress -->
    <div class="w-full bg-white/20 rounded-full h-3 mb-6">
      <div class="bg-gradient-to-r from-green-400 via-yellow-400 to-pink-500 h-3 rounded-full transition-all duration-700 animate-pulse" style="width: 70%"></div>
    </div>
    <p class="text-sm mb-8 text-white/70">Progress: 70% Complete</p>

    <!-- Notify Form -->
    <form class="flex flex-col sm:flex-row gap-3 justify-center">
      <input type="email" placeholder="Enter your email" 
        class="px-4 py-3 rounded-xl bg-white/20 text-white placeholder-white/70 focus:outline-none flex-1">
      <button class="px-6 py-3 rounded-xl bg-gradient-to-r from-pink-500 to-purple-600 font-bold hover:scale-105 transition">
        Notify Me
      </button>
    </form>
  </div>

  <!-- Social Links -->
  <div class="flex space-x-8 mt-10">
    <a href="https://github.com/yourusername" target="_blank" class="glow transition rounded-full p-3">
      <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" class="w-8 h-8" />
    </a>
    <a href="mailto:contact@lipataka.com" class="glow transition rounded-full p-3">
      <svg xmlns="http://www.w3.org/2000/svg" class="w-8 h-8" fill="white" viewBox="0 0 24 24"><path d="M12 13.065 1.5 6h21L12 13.065zm0 2.11L1.5 8.106V18h21V8.106L12 15.175z"/></svg>
    </a>
    <a href="#" class="glow transition rounded-full p-3">
      <svg xmlns="http://www.w3.org/2000/svg" class="w-8 h-8" fill="white" viewBox="0 0 24 24"><path d="M22.54 6.42c-.79.35-1.63.59-2.52.7a4.48 4.48 0 0 0 1.98-2.48c-.86.51-1.8.87-2.8 1.07a4.49 4.49 0 0 0-7.65 4.1 12.75 12.75 0 0 1-9.26-4.7 4.49 4.49 0 0 0 1.39 6 4.45 4.45 0 0 1-2.03-.56v.06a4.49 4.49 0 0 0 3.6 4.4 4.47 4.47 0 0 1-2.02.08 4.5 4.5 0 0 0 4.2 3.12A9 9 0 0 1 2 19.54a12.73 12.73 0 0 0 6.91 2.03c8.3 0 12.84-6.87 12.84-12.83 0-.2 0-.39-.01-.58a9.1 9.1 0 0 0 2.21-2.32z"/></svg>
    </a>
  </div>

  <!-- Footer -->
  <footer class="mt-16 text-sm text-white/70">
    © <span id="year"></span> Lipataka. All Rights Reserved.
  </footer>

  <script>
    document.getElementById("year").innerText = new Date().getFullYear();
  </script>
</body>
</html>
