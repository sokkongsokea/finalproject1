<!DOCTYPE html>
<html lang="en" class="light">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Portfolio | Light & Dark Mode</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
      tailwind.config = {
        darkMode: 'class',
        theme: {
          extend: {
            colors: {
              'dark-bg': '#0f172a',
              'dark-card': '#1e293b',
              'primary-gold': '#c5a059',
            }
          }
        }
      }
    </script>
    <style>
      @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap');
      body {
        font-family: 'Inter', sans-serif;
        transition: background-color 0.3s, color 0.3s;
      }
      .scroll-mt-24 {
        scroll-margin-top: 6rem;
      }
    </style>
  </head>
  <body class="bg-gray-50 dark:bg-dark-bg text-gray-900 dark:text-gray-100 transition-colors duration-300">
    
    <!-- Navigation -->
    <nav class="bg-white/80 dark:bg-slate-900/80 backdrop-blur-md border-b border-gray-200 dark:border-gray-800 p-4 sticky top-0 z-50 transition-colors">
      <div class="container mx-auto flex flex-col lg:flex-row justify-between items-center px-4">
        <div class="text-gray-900 dark:text-white font-bold text-3xl mb-4 lg:mb-0 hover:text-orange-600 transition-colors cursor-pointer">
          Portfolio
        </div>

        <div class="flex items-center space-x-4 lg:space-x-8">
          <div class="hidden md:flex space-x-6 font-medium text-lg">
            <a href="#home" class="hover:text-orange-600 transition-colors">Home</a>
            <a href="#about" class="hover:text-orange-600 transition-colors">About</a>
            <a href="#Projects" class="hover:text-orange-600 transition-colors">Projects</a>
            <a href="#contact" class="hover:text-orange-600 transition-colors">Contact</a>
          </div>

          <!-- Theme Toggle Button -->
          <button id="theme-toggle" class="p-2.5 rounded-xl bg-gray-100 dark:bg-slate-800 text-gray-500 dark:text-gray-400 hover:bg-gray-200 dark:hover:bg-slate-700 transition-all focus:outline-none border border-gray-200 dark:border-gray-700">
            <svg id="theme-toggle-dark-icon" class="hidden w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M17.293 13.293A8 8 0 016.707 2.707a8.001 8.001 0 1010.586 10.586z"></path></svg>
            <svg id="theme-toggle-light-icon" class="hidden w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path d="M10 2a1 1 0 011 1v1a1 1 0 11-2 0V3a1 1 0 011-1zm4 8a4 4 0 11-8 0 4 4 0 018 0zm-.464 4.95l.707.707a1 1 0 001.414-1.414l-.707-.707a1 1 0 00-1.414 1.414zm2.12-10.607a1 1 0 010 1.414l-.706.707a1 1 0 11-1.414-1.414l.707-.707a1 1 0 011.414 0zM17 11a1 1 0 100-2h-1a1 1 0 100 2h1zm-7 4a1 1 0 011 1v1a1 1 0 11-2 0v-1a1 1 0 011-1zM5.05 6.464A1 1 0 106.465 5.05l-.708-.707a1 1 0 00-1.414 1.414l.707.707zm1.414 8.486l-.707.707a1 1 0 01-1.414-1.414l.707-.707a1 1 0 011.414 1.414zM4 11a1 1 0 100-2H3a1 1 0 000 2h1z" fill-rule="evenodd" clip-rule="evenodd"></path></svg>
          </button>
        </div>
      </div>
    </nav>

    <!-- Hero Section (Home) -->
    <header id="home" class="relative min-h-[85vh] flex items-center justify-center text-center text-white scroll-mt-24 overflow-hidden">
      <img src="https://images.unsplash.com/photo-1497215728101-856f4ea42174?auto=format&fit=crop&q=80&w=1920" class="absolute inset-0 w-full h-full object-cover brightness-[0.4] dark:brightness-[0.25] transition-all" alt="Workspace" />
      <div class="relative z-10 px-6 max-w-4xl animate-fadeIn">
        <h1 class="text-6xl md:text-8xl font-bold mb-6 tracking-tight">Digital Architect</h1>
        <p class="text-xl md:text-2xl mb-12 font-light text-gray-300">Transforming complex ideas into elegant digital solutions with a focus on user experience and performance.</p>
        <div class="flex flex-col md:flex-row space-y-4 md:space-y-0 md:space-x-6 justify-center">
          <a href="#Projects" class="bg-orange-600 text-white px-10 py-4 rounded-full font-bold hover:bg-orange-700 transition transform hover:scale-105 shadow-xl">My Work</a>
          <a href="#about" class="bg-white/10 backdrop-blur-md border border-white/20 text-white px-10 py-4 rounded-full font-bold hover:bg-white/20 transition transform hover:scale-105">Learn More</a>
        </div>
      </div>
    </header>

    <!-- About Section -->
    <section id="about" class="py-32 px-6 max-w-7xl mx-auto scroll-mt-24">
      <div class="grid lg:grid-cols-2 gap-20 items-center">
        <div class="relative">
          <div class="absolute inset-0 bg-orange-600/20 blur-3xl -z-10 rounded-full"></div>
          <img src="https://images.unsplash.com/photo-1550966841-3ee4ad05f039?auto=format&fit=crop&q=80&w=1000" class="rounded-3xl shadow-2xl relative z-10 grayscale hover:grayscale-0 transition-all duration-1000" alt="About Image" />
          <div class="absolute -bottom-10 -right-10 w-40 h-40 bg-orange-600 rounded-3xl -z-0 hidden lg:block opacity-20"></div>
        </div>
        <div class="space-y-8">
          <h2 class="text-5xl font-bold leading-tight">Crafting Experiences That Matter.</h2>
          <p class="text-xl text-gray-600 dark:text-gray-400 leading-relaxed">
            With over 12 years of experience in the industry, I've had the privilege of working with global brands to build digital products that people love to use.
          </p>
          <p class="text-xl text-gray-600 dark:text-gray-400 leading-relaxed">
            I specialize in cross-platform development, UI/UX design, and scalable system architecture, ensuring every pixel and line of code serves a purpose.
          </p>
          <div class="grid grid-cols-2 gap-8 pt-8 border-t border-gray-200 dark:border-gray-800">
            <div>
              <span class="block text-4xl font-bold text-orange-600">50+</span>
              <span class="text-sm uppercase tracking-widest font-semibold opacity-60">Projects Completed</span>
            </div>
            <div>
              <span class="block text-4xl font-bold text-orange-600">12</span>
              <span class="text-sm uppercase tracking-widest font-semibold opacity-60">Global Awards</span>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Projects (Grid Section) -->
    <section id="Projects" class="py-32 bg-gray-100 dark:bg-slate-900/50 px-6 scroll-mt-24 transition-colors">
      <div class="max-w-7xl mx-auto">
        <div class="text-center mb-20">
          <h2 class="text-5xl font-bold mb-6">Recent Projects</h2>
          <div class="h-1.5 w-24 bg-orange-600 mx-auto rounded-full"></div>
        </div>
        
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-12">
          <!-- Card Template Applied -->
          <script>
            const products = [
              { name: "Lumina App", desc: "A sleek dashboard for real-time analytics and user behavior tracking.", img: "https://images.unsplash.com/photo-1646753522408-077ef9839300?auto=format&fit=crop&w=500&q=60" },
              { name: "EcoCommerce", desc: "A sustainable shopping platform with minimalist design principles.", img: "https://images.unsplash.com/photo-1651950519238-15835722f8bb?auto=format&fit=crop&w=500&q=60" },
              { name: "Pulse Design", desc: "Custom icon library and design system for tech startups.", img: "https://images.unsplash.com/photo-1651950537598-373e4358d320?auto=format&fit=crop&w=500&q=60" },
              { name: "Nebula OS", desc: "Conceptual operating system interface focused on fluid animations.", img: "https://images.unsplash.com/photo-1651950540805-b7c71869e689?auto=format&fit=crop&w=500&q=60" },
              { name: "Zenith Sound", desc: "High-fidelity audio streaming app for audiophiles.", img: "https://images.unsplash.com/photo-1649261191624-ca9f79ca3fc6?auto=format&fit=crop&w=500&q=60" },
              { name: "Titan UI", desc: "An open-source component library for React and Tailwind.", img: "https://images.unsplash.com/photo-1649261191606-cb2496e97eee?auto=format&fit=crop&w=500&q=60" }
            ];

            products.forEach(p => {
              document.write(`
                <div class="group bg-white dark:bg-slate-800 rounded-[2rem] overflow-hidden shadow-sm hover:shadow-2xl transition-all duration-500 border border-gray-100 dark:border-gray-700">
                  <div class="h-72 overflow-hidden relative">
                    <img src="${p.img}" class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-700" alt="${p.name}" />
                    <div class="absolute inset-0 bg-gradient-to-t from-black/60 to-transparent opacity-0 group-hover:opacity-100 transition-opacity flex items-end p-8">
                      <span class="text-white font-bold tracking-widest uppercase text-xs">View Project</span>
                    </div>
                  </div>
                  <div class="p-8">
                    <h3 class="text-2xl font-bold mb-3 group-hover:text-orange-600 transition-colors">${p.name}</h3>
                    <p class="text-gray-500 dark:text-gray-400 mb-6 leading-relaxed">${p.desc}</p>
                    <a href="#" class="inline-flex items-center text-orange-600 font-bold hover:underline">
                      Explore Details
                      <svg class="w-4 h-4 ml-2" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="3" d="M9 5l7 7-7 7"></path></svg>
                    </a>
                  </div>
                </div>
              `);
            });
          </script>
        </div>
      </div>
    </section>

    <!-- Contact & Footer Section -->
    <footer id="contact" class="bg-gray-900 dark:bg-black text-white py-32 px-6 scroll-mt-24 transition-colors">
      <div class="max-w-7xl mx-auto">
        <div class="grid lg:grid-cols-2 gap-24 mb-24">
          <div class="space-y-10">
            <h2 class="text-6xl font-bold leading-tight">Let's Build Something Great Together.</h2>
            <p class="text-2xl text-gray-400 font-light">Available for freelance projects and consulting. Shoot me an email or find me on social media.</p>
            <div class="space-y-6 text-xl">
              <p class="flex items-center group"><span class="w-12 h-12 bg-gray-800 rounded-full flex items-center justify-center mr-6 group-hover:bg-orange-600 transition-colors">📍</span> 123 Digital Square, Blue City, 90210</p>
              <p class="flex items-center group"><span class="w-12 h-12 bg-gray-800 rounded-full flex items-center justify-center mr-6 group-hover:bg-orange-600 transition-colors">✉️</span> hello@example.com</p>
            </div>
            <div class="flex space-x-6 pt-6">
              <a href="#" class="w-14 h-14 bg-gray-800 rounded-2xl flex items-center justify-center hover:bg-orange-600 transition-all transform hover:-translate-y-2 font-bold">IG</a>
              <a href="#" class="w-14 h-14 bg-gray-800 rounded-2xl flex items-center justify-center hover:bg-orange-600 transition-all transform hover:-translate-y-2 font-bold">TW</a>
              <a href="#" class="w-14 h-14 bg-gray-800 rounded-2xl flex items-center justify-center hover:bg-orange-600 transition-all transform hover:-translate-y-2 font-bold">LN</a>
            </div>
          </div>

          <form class="space-y-6 bg-white/5 p-12 rounded-[3rem] backdrop-blur-sm border border-white/10 shadow-2xl">
            <h3 class="text-3xl font-bold mb-8">Send a Message</h3>
            <div class="space-y-4">
              <input type="text" placeholder="Full Name" class="w-full p-5 bg-gray-800/50 border border-gray-700 rounded-2xl outline-none focus:border-orange-600 focus:ring-2 focus:ring-orange-600/20 transition-all" />
              <input type="email" placeholder="Email Address" class="w-full p-5 bg-gray-800/50 border border-gray-700 rounded-2xl outline-none focus:border-orange-600 focus:ring-2 focus:ring-orange-600/20 transition-all" />
              <textarea placeholder="Tell me about your project" rows="4" class="w-full p-5 bg-gray-800/50 border border-gray-700 rounded-2xl outline-none focus:border-orange-600 focus:ring-2 focus:ring-orange-600/20 transition-all"></textarea>
              <button type="button" class="w-full bg-orange-600 py-5 rounded-2xl font-bold hover:bg-orange-700 transition transform hover:scale-[1.02] shadow-xl text-xl">Get in Touch</button>
            </div>
          </form>
        </div>
        
        <div class="pt-16 border-t border-gray-800 flex flex-col md:flex-row justify-between items-center opacity-60 text-sm tracking-widest uppercase">
          <p>&copy; 2026 BrandName Portfolio. All rights reserved.</p>
          <div class="flex space-x-12 mt-8 md:mt-0">
            <a href="#" class="hover:text-orange-600 transition">Privacy</a>
            <a href="#" class="hover:text-orange-600 transition">Cookies</a>
            <a href="#" class="hover:text-orange-600 transition">Terms</a>
          </div>
        </div>
      </div>
    </footer>

    <script>
      // Theme Toggle Script
      const themeToggleBtn = document.getElementById('theme-toggle');
      const darkIcon = document.getElementById('theme-toggle-dark-icon');
      const lightIcon = document.getElementById('theme-toggle-light-icon');
      const html = document.documentElement;

      // Initial Theme Check
      if (localStorage.getItem('color-theme') === 'dark' || (!('color-theme' in localStorage) && window.matchMedia('(prefers-color-scheme: dark)').matches)) {
        html.classList.add('dark');
        lightIcon.classList.remove('hidden');
      } else {
        html.classList.remove('dark');
        darkIcon.classList.remove('hidden');
      }

      themeToggleBtn.addEventListener('click', () => {
        html.classList.toggle('dark');
        const isDark = html.classList.contains('dark');
        localStorage.setItem('color-theme', isDark ? 'dark' : 'light');
        
        darkIcon.classList.toggle('hidden');
        lightIcon.classList.toggle('hidden');
      });
    </script>
  </body>
</html>


