<script>
  import SectionLabel from './SectionLabel.svelte';
</script>

<section class="bg-[#F5F1EB] px-6 py-24">
  <div class="max-w-[1400px] mx-auto grid grid-cols-1 lg:grid-cols-12 gap-12">
    <div class="lg:col-span-3">
      <SectionLabel label="Why Brave Studio" />
    </div>
    
    <div class="lg:col-span-9 grid grid-cols-1 md:grid-cols-2 gap-16">
      <div>
        <h2 class="font-serif text-3xl md:text-4xl leading-tight text-gray-900 mb-6" style="font-family: 'Noe Display', serif;">
          Built for creative agencies and production studios
        </h2>
        <p class="text-gray-600 leading-relaxed">
          Brave Studio streamlines everything from brief to final export. No more messy handoffs, version nightmares, or chasing feedback. Just intuitive tools and real-time collaboration that keep ideas moving.
        </p>
      </div>
      
      <div class="flex flex-col gap-8 justify-center">
        <div class="flex flex-col gap-2">
          <h3 class="font-medium text-gray-900">AI-powered generation</h3>
          <p class="text-sm text-gray-500 leading-relaxed">Generate high-quality video assets in seconds, ready for editing or approval</p>
        </div>
        <div class="flex flex-col gap-2">
          <h3 class="font-medium text-gray-900">Collaborative editing</h3>
          <p class="text-sm text-gray-500 leading-relaxed">Bring teams, clients, and feedback into one shared space</p>
        </div>
        <div class="flex flex-col gap-2">
          <h3 class="font-medium text-gray-900">Fast exports</h3>
          <p class="text-sm text-gray-500 leading-relaxed">Final assets export in minutes—perfect for fast-paced campaigns</p>
        </div>
      </div>
    </div>
  </div>
</section>
