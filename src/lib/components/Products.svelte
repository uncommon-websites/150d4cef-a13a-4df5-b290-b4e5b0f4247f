<script>
  import SectionLabel from './SectionLabel.svelte';
</script>

<section class="bg-[#F5F1EB] px-6 py-24 border-t border-[#E1DED8]">
  <div class="max-w-[1400px] mx-auto grid grid-cols-1 lg:grid-cols-12 gap-12">
    <div class="lg:col-span-3">
      <SectionLabel label="What's Inside" />
    </div>
    
    <div class="lg:col-span-9">
      <div class="mb-16">
        <h2 class="font-serif text-4xl md:text-5xl text-gray-900 mb-2" style="font-family: 'Noe Display', serif;">
          AI asset generation
        </h2>
        <h2 class="font-serif text-4xl md:text-5xl text-gray-400" style="font-family: 'Noe Display', serif;">
          meets collaborative design tools
        </h2>
      </div>

      <div class="grid gap-0 border-t border-[#E1DED8]">
        <!-- Item 1 -->
        <a href="/" class="group grid grid-cols-1 md:grid-cols-12 gap-6 py-10 border-b border-[#E1DED8] hover:bg-white transition-colors px-4 -mx-4">
          <div class="md:col-span-4">
            <div class="text-xs text-gray-400 mb-1">Generate in seconds</div>
            <h3 class="text-2xl font-medium text-gray-900">AI Asset Generation</h3>
          </div>
          <div class="md:col-span-7">
            <p class="text-gray-600 leading-relaxed">
              Upload a clip or start from scratch—Brave Studio uses generative tools to create usable media instantly. From characters to scenes, bring your vision to life in less time.
            </p>
          </div>
          <div class="md:col-span-1 flex justify-end items-start pt-2">
            <svg class="w-6 h-6 text-gray-400 group-hover:text-secondary-700 transform group-hover:translate-x-1 transition-all" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 8l4 4m0 0l-4 4m4-4H3"></path></svg>
          </div>
        </a>

        <!-- Item 2 -->
        <a href="/" class="group grid grid-cols-1 md:grid-cols-12 gap-6 py-10 border-b border-[#E1DED8] hover:bg-white transition-colors px-4 -mx-4">
          <div class="md:col-span-4">
            <div class="text-xs text-gray-400 mb-1">Work together in real time</div>
            <h3 class="text-2xl font-medium text-gray-900">Collaborative Design Tools</h3>
          </div>
          <div class="md:col-span-7">
            <p class="text-gray-600 leading-relaxed">
              Work together in real time, review frame by frame, and make approved changes without leaving the platform. Everything stays synced, on track, and easy to find.
            </p>
          </div>
          <div class="md:col-span-1 flex justify-end items-start pt-2">
            <svg class="w-6 h-6 text-gray-400 group-hover:text-secondary-700 transform group-hover:translate-x-1 transition-all" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 8l4 4m0 0l-4 4m4-4H3"></path></svg>
          </div>
        </a>
      </div>
    </div>
  </div>
</section>
