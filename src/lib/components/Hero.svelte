<script>
    // Hero Component
</script>

<section class="pt-32 pb-16 md:pt-40 md:pb-24 bg-gray-50 relative overflow-hidden font-sans">
    <!-- Grid Background Pattern -->
    <div class="absolute inset-0 z-0 opacity-[0.4]" 
         style="background-image: linear-gradient(#e5e7eb 1px, transparent 1px), linear-gradient(90deg, #e5e7eb 1px, transparent 1px); background-size: 40px 40px;">
    </div>

    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10 flex flex-col items-center text-center">
        
        <!-- Headline -->
        <h1 class="text-5xl md:text-7xl lg:text-8xl font-serif-display text-gray-900 leading-[1.1] tracking-tight mb-6 max-w-5xl mx-auto">
            Never write <br class="hidden md:block" />
            another post
        </h1>

        <!-- Subheadline -->
        <p class="text-lg md:text-xl text-gray-600 max-w-2xl mx-auto mb-10 leading-relaxed">
            V30 transforms social media chaos into consistent growth through autonomous AI agents managing your strategy, creation, and publishing.
        </p>

        <!-- CTA -->
        <div class="mb-16 flex flex-col sm:flex-row gap-4 items-center">
            <a href="#" class="inline-flex items-center justify-center px-8 py-4 border border-transparent text-base font-medium rounded-full text-white bg-gray-900 hover:bg-gray-800 transition-all shadow-lg hover:shadow-xl transform hover:-translate-y-0.5">
                Start Free Trial
                <svg class="w-5 h-5 ml-2" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14 5l7 7m0 0l-7 7m7-7H3"></path></svg>
            </a>
            <p class="text-sm text-gray-500">No credit card required • 3 credits free</p>
        </div>

        <!-- Product Dashboard Mockup -->
        <div class="w-full max-w-5xl mx-auto rounded-lg overflow-hidden shadow-2xl bg-white border border-gray-200 relative">
            <!-- Browser Chrome -->
            <div class="bg-gray-100 border-b border-gray-200 px-4 py-3 flex items-center gap-2">
                <div class="flex gap-1.5">
                    <div class="w-3 h-3 rounded-full bg-red-400"></div>
                    <div class="w-3 h-3 rounded-full bg-yellow-400"></div>
                    <div class="w-3 h-3 rounded-full bg-green-400"></div>
                </div>
                <div class="flex-1 flex justify-center">
                    <div class="bg-white rounded px-4 py-1 text-xs text-gray-600 border border-gray-200">app.v30.ai</div>
                </div>
            </div>

            <!-- Dashboard Content -->
            <div class="bg-gradient-to-br from-gray-50 to-white p-8">
                <!-- Header -->
                <div class="mb-6 flex items-center justify-between">
                    <div>
                        <h3 class="text-2xl font-serif-display text-gray-900">30-Day Content Calendar</h3>
                        <p class="text-sm text-gray-500 mt-1">Next 7 days • LinkedIn & X</p>
                    </div>
                    <div class="flex items-center gap-2 text-sm">
                        <span class="px-3 py-1.5 bg-green-100 text-green-700 rounded-full font-medium">+127 followers</span>
                        <span class="px-3 py-1.5 bg-blue-100 text-blue-700 rounded-full font-medium">15% growth</span>
                    </div>
                </div>

                <!-- Calendar Grid -->
                <div class="grid grid-cols-7 gap-3">
                    {#each Array(7) as _, i}
                    <div class="bg-white rounded-lg border border-gray-200 p-3 hover:shadow-md transition-shadow">
                        <div class="text-xs font-bold text-gray-400 mb-2">
                            {['MON', 'TUE', 'WED', 'THU', 'FRI', 'SAT', 'SUN'][i]}
                        </div>
                        <div class="space-y-2">
                            {#if i < 5}
                            <div class="bg-blue-50 border border-blue-200 rounded p-2 text-[10px]">
                                <div class="flex items-center gap-1 mb-1">
                                    <svg class="w-3 h-3 text-blue-600" fill="currentColor" viewBox="0 0 24 24"><path d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.764s.784-1.764 1.75-1.764 1.75.79 1.75 1.764-.783 1.764-1.75 1.764zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z"/></svg>
                                    <span class="font-bold text-blue-900">LinkedIn</span>
                                </div>
                                <p class="text-gray-700 line-clamp-2">AI agents are changing how...</p>
                            </div>
                            {/if}
                            {#if i % 2 === 0 && i < 6}
                            <div class="bg-gray-50 border border-gray-200 rounded p-2 text-[10px]">
                                <div class="flex items-center gap-1 mb-1">
                                    <svg class="w-3 h-3 text-gray-900" fill="currentColor" viewBox="0 0 24 24"><path d="M18.244 2.25h3.308l-7.227 8.26 8.502 11.24H16.17l-5.214-6.817L4.99 21.75H1.68l7.73-8.835L1.254 2.25H8.08l4.713 6.231zm-1.161 17.52h1.833L7.084 4.126H5.117z"/></svg>
                                    <span class="font-bold text-gray-900">X</span>
                                </div>
                                <p class="text-gray-700 line-clamp-2">Just shipped a new feature...</p>
                            </div>
                            {/if}
                        </div>
                    </div>
                    {/each}
                </div>
            </div>
        </div>
    </div>
</section>
