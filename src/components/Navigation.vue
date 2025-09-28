<script setup></script>

<template>
  <!-- Navigation -->
  <nav
    class="bg-secondary/80 backdrop-blur-md sticky top-0 z-50 border-b border-gray-700"
  >
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex items-center justify-between h-16">
        <div class="flex items-center">
          <div class="flex-shrink-0">
            <span class="text-accent font-mono text-xl font-bold">CommercialSky1174</span>
          </div>
          <div class="hidden md:block">
            <div class="ml-10 flex items-baseline space-x-4">
              <a
                href="#"
                class="text-white px-3 py-2 rounded-md text-sm font-medium hover:text-accent transition"
                >Home</a
              >
              <a
                href="#blog"
                class="text-gray-300 hover:text-white px-3 py-2 rounded-md text-sm font-medium transition"
                >Blog</a
              >
              <a
                href="#contact"
                class="text-gray-300 hover:text-white px-3 py-2 rounded-md text-sm font-medium transition"
                >Contact</a
              >
            </div>
          </div>
        </div>
        <div class="hidden md:block">
          <div class="ml-4 flex items-center md:ml-6">
            <button
              class="bg-accent text-primary px-4 py-2 rounded-md text-sm font-mono font-bold hover:bg-opacity-90 transition"
            >
              Submit Proposal
            </button>
          </div>
        </div>
        <div class="-mr-2 flex md:hidden">
          <button
            type="button"
            class="inline-flex items-center justify-center p-2 rounded-md text-gray-400 hover:text-white hover:bg-gray-700 focus:outline-none"
          >
            <i data-feather="menu"></i>
          </button>
        </div>
      </div>
    </div>
  </nav>
</template>
