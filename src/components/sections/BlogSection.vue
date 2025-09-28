<script setup></script>

<template>
  <section id="blog" class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 mb-20">
    <h2 class="text-3xl font-bold text-white mb-8 flex items-center">
      <i data-feather="message-square" class="mr-3 text-accent"></i> Latest Updates
    </h2>

    <div class="space-y-6">
      <!-- Blog Post 1 -->
      <div
        class="post-card bg-secondary rounded-lg p-6 transition duration-300 ease-in-out"
      >
        <div class="flex justify-between items-start mb-2">
          <span class="text-sm font-mono text-accent">2023-11-15</span>
          <span class="text-xs bg-gray-700 text-gray-300 px-2 py-1 rounded"
            >Development</span
          >
        </div>
        <p class="text-gray-300 mb-4">
          Just deployed the new API gateway with 40% faster response times. Benchmark
          results look promising!
        </p>
        <div class="flex items-center text-gray-500 text-sm">
          <i data-feather="clock" class="w-4 h-4 mr-1"></i>
          <span>2 min read</span>
        </div>
      </div>

      <!-- Blog Post 2 -->
      <div
        class="post-card bg-secondary rounded-lg p-6 transition duration-300 ease-in-out"
      >
        <div class="flex justify-between items-start mb-2">
          <span class="text-sm font-mono text-accent">2023-11-12</span>
          <span class="text-xs bg-gray-700 text-gray-300 px-2 py-1 rounded"
            >Announcement</span
          >
        </div>
        <p class="text-gray-300 mb-4">
          We're now accepting project proposals for Q1 2024. Priority given to open-source
          and innovative ideas.
        </p>
        <div class="flex items-center text-gray-500 text-sm">
          <i data-feather="clock" class="w-4 h-4 mr-1"></i>
          <span>1 min read</span>
        </div>
      </div>

      <!-- Blog Post 3 -->
      <div
        class="post-card bg-secondary rounded-lg p-6 transition duration-300 ease-in-out"
      >
        <div class="flex justify-between items-start mb-2">
          <span class="text-sm font-mono text-accent">2023-11-08</span>
          <span class="text-xs bg-gray-700 text-gray-300 px-2 py-1 rounded"
            >Milestone</span
          >
        </div>
        <p class="text-gray-300 mb-4">
          Reached 60% of our funding goal! Huge thanks to everyone who contributed. New
          stretch goals coming soon.
        </p>
        <div class="flex items-center text-gray-500 text-sm">
          <i data-feather="clock" class="w-4 h-4 mr-1"></i>
          <span>1 min read</span>
        </div>
      </div>
    </div>

    <div class="mt-8 text-center">
      <button
        class="border border-gray-600 text-white px-6 py-2 rounded-md font-medium hover:bg-gray-800 transition"
      >
        Load More
      </button>
    </div>
  </section>
</template>
