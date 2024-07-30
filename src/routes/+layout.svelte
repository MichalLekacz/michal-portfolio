<script>
    import "../app.css";
  </script>
  
  <nav class="bg-blue-950">
    <div class="max-w-screen-lg mx-auto px-4 sm:px-6 lg:px-8 flex items-center justify-between h-16">
      <!-- Logo Section -->
      <div class="flex items-center">
        <span class="text-blue-400 ml-2 text-xl font-semibold ">michallekacz<span class="text-indigo-400">.</span>info</span>
      </div>
      <!-- Navigation Menu -->
      <div class="hidden md:flex space-x-4">
        <a href="/" class="text-blue-200 hover:bg-indigo-900 hover:text-indigo-300 px-3 py-2 rounded-md text-sm font-medium">Home</a>
        <a href="/about" class="text-blue-200 hover:bg-indigo-900 hover:text-indigo-300 px-3 py-2 rounded-md text-sm font-medium">About</a>
        <a href="/projects" class="text-blue-200 hover:bg-indigo-900 hover:text-indigo-300 px-3 py-2 rounded-md text-sm font-medium">Experience</a>
        <a href="/projects" class="text-blue-200 hover:bg-indigo-900 hover:text-indigo-300 px-3 py-2 rounded-md text-sm font-medium">Projects</a>
        <a href="/contact" class="text-blue-200 hover:bg-indigo-900 hover:text-indigo-300 px-3 py-2 rounded-md text-sm font-medium">Contact</a>
      </div>
    </div>
  </nav>
  
  <main>
    <slot></slot>
  </main>