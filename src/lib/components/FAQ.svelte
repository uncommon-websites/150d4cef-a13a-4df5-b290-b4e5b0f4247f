<script lang="ts">
  import { slide } from 'svelte/transition';
  
  interface FAQItem {
    question: string;
    answer: string;
  }

  const faqs: FAQItem[] = [
    { question: "What types of video assets can Brave Studio generate?", answer: "Brave Studio can generate a wide range of video assets including characters, scenes, backgrounds, effects, and transitions. Our AI tools work with your existing footage or create assets from scratch based on your creative direction." },
    { question: "Can I use Brave Studio with my existing workflow or tools?", answer: "Yes. Brave Studio integrates seamlessly with industry-standard tools like Adobe Premiere, After Effects, and Final Cut Pro. You can export assets in multiple formats and maintain your preferred editing workflow." },
    { question: "How does client feedback work inside the platform?", answer: "Clients can review work directly in Brave Studio with frame-by-frame commenting, timestamp annotations, and approval workflows. All feedback is centralized and synced in real-time, eliminating email chains and version confusion." },
    { question: "Is there a way to track version history on collaborative edits?", answer: "Absolutely. Every edit is automatically versioned and saved. You can review the complete history, compare versions side-by-side, and restore previous iterations at any time." },
    { question: "Is Brave Studio secure enough for client and proprietary work?", answer: "Security is our priority. All assets are encrypted in transit and at rest, with enterprise-grade access controls, SSO support, and compliance with industry standards including SOC 2 and GDPR." },
    { question: "Do you offer features for indie game developers or in-game content?", answer: "Yes. Brave Studio supports game developers with specialized tools for creating in-game cinematics, character animations, and promotional content. Our AI generation tools are optimized for game asset workflows." },
    { question: "What does onboarding look like for creative teams?", answer: "We provide dedicated onboarding with training sessions tailored to your team's workflow. Most teams are fully productive within a week, and we offer ongoing support through our success team and community resources." }
  ];

  let openIndex: number | null = null;

  function toggle(index: number) {
    openIndex = openIndex === index ? null : index;
  }
</script>

<section class="bg-[#F5F1EB] px-6 py-24">
  <div class="max-w-[1400px] mx-auto grid grid-cols-1 lg:grid-cols-12 gap-12">
    <div class="lg:col-span-4">
      <h2 class="font-serif text-4xl text-gray-900 mb-6" style="font-family: 'Noe Display', serif;">
        Frequently asked questions
      </h2>
      <a href="/" class="text-sm text-gray-900 border-b border-gray-400 pb-0.5 hover:border-secondary-700 transition-colors">See all support</a>
    </div>
    
    <div class="lg:col-span-8">
      <div class="border-t border-[#E1DED8]">
        {#each faqs as faq, i}
          <div class="border-b border-[#E1DED8]">
            <button 
              class="w-full py-6 flex justify-between items-center text-left hover:bg-white/50 transition-colors"
              on:click={() => toggle(i)}
            >
              <span class="text-lg text-gray-800">{faq.question}</span>
              <span class="text-2xl font-light text-gray-400 ml-4">
                {openIndex === i ? '−' : '+'}
              </span>
            </button>
            {#if openIndex === i}
              <div transition:slide class="pb-6 text-gray-600 leading-relaxed">
                {faq.answer}
              </div>
            {/if}
          </div>
        {/each}
      </div>
    </div>
  </div>
</section>
