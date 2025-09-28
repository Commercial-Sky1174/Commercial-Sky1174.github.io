<script setup></script>

<template>
  <section id="contact" class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 mb-20">
    <div class="bg-secondary rounded-xl p-8 shadow-lg">
      <h2 class="text-3xl font-bold text-white mb-6 flex items-center">
        <i data-feather="send" class="mr-3 text-accent"></i> Submit Proposal
      </h2>

      <form class="space-y-6">
        <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
          <div>
            <label for="name" class="block text-sm font-medium text-gray-300 mb-1"
              >Your Name</label
            >
            <input
              type="text"
              id="name"
              class="w-full bg-gray-700 border border-gray-600 rounded-md px-4 py-2 text-white focus:outline-none focus:ring-2 focus:ring-accent focus:border-transparent"
              placeholder="John Doe"
            />
          </div>
          <div>
            <label for="email" class="block text-sm font-medium text-gray-300 mb-1"
              >Email Address</label
            >
            <input
              type="email"
              id="email"
              class="w-full bg-gray-700 border border-gray-600 rounded-md px-4 py-2 text-white focus:outline-none focus:ring-2 focus:ring-accent focus:border-transparent"
              placeholder="you@example.com"
            />
          </div>
        </div>

        <div>
          <label for="project" class="block text-sm font-medium text-gray-300 mb-1"
            >Project Title</label
          >
          <input
            type="text"
            id="project"
            class="w-full bg-gray-700 border border-gray-600 rounded-md px-4 py-2 text-white focus:outline-none focus:ring-2 focus:ring-accent focus:border-transparent"
            placeholder="My Awesome Project"
          />
        </div>

        <div>
          <label for="description" class="block text-sm font-medium text-gray-300 mb-1"
            >Project Description</label
          >
          <textarea
            id="description"
            rows="5"
            class="w-full bg-gray-700 border border-gray-600 rounded-md px-4 py-2 text-white focus:outline-none focus:ring-2 focus:ring-accent focus:border-transparent"
            placeholder="Describe your project in detail..."
          ></textarea>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
          <div>
            <label for="budget" class="block text-sm font-medium text-gray-300 mb-1"
              >Estimated Budget (USDT)</label
            >
            <input
              type="number"
              id="budget"
              class="w-full bg-gray-700 border border-gray-600 rounded-md px-4 py-2 text-white focus:outline-none focus:ring-2 focus:ring-accent focus:border-transparent"
              placeholder="5000"
            />
          </div>
          <div>
            <label for="timeline" class="block text-sm font-medium text-gray-300 mb-1"
              >Estimated Timeline</label
            >
            <select
              id="timeline"
              class="w-full bg-gray-700 border border-gray-600 rounded-md px-4 py-2 text-white focus:outline-none focus:ring-2 focus:ring-accent focus:border-transparent"
            >
              <option>1-3 months</option>
              <option>3-6 months</option>
              <option>6-12 months</option>
              <option>1+ years</option>
            </select>
          </div>
        </div>

        <div class="pt-4">
          <button
            type="submit"
            class="w-full bg-accent text-primary px-6 py-3 rounded-md font-mono font-bold hover:bg-opacity-90 transition"
          >
            Submit Proposal
          </button>
        </div>
      </form>
    </div>
  </section>
</template>
