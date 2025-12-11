<script>
    // No script logic needed for this static recreation yet
</script>

<section class="py-20 bg-white font-sans">
    <div class="max-w-7xl mx-auto px-4 text-center">
        <span class="text-[10px] font-bold text-gray-500 uppercase tracking-widest border border-gray-200 px-3 py-1.5 rounded-full bg-gray-50">The V30 Platform</span>
        <h2 class="mt-8 text-5xl md:text-7xl font-serif-display text-gray-900 leading-tight">Your entire <br/> marketing team, <br/> in one agent</h2>
    </div>
    
    <!-- Tabbed interface image area -->
    <div class="max-w-7xl mx-auto mt-16 px-4">
        <div class="border border-gray-200 rounded-xl overflow-hidden shadow-sm bg-white grid md:grid-cols-12 min-h-[600px]">
             <div class="md:col-span-4 p-8 md:p-12 border-r border-gray-200 flex flex-col justify-center">
                 <h3 class="text-3xl font-serif-display mb-4">30 days of content, planned in minutes</h3>
                 <p class="text-gray-600 text-base leading-relaxed mb-8">V30 analyzes your business, audience, and top-performing content to create a complete 30-day content calendar. Every post is strategically timed and optimized for maximum engagement. Just review, approve, and watch your audience grow.</p>
                 <div>
                    <button class="text-sm font-bold border-b border-gray-300 pb-0.5 hover:border-gray-900 transition-colors">Learn More -></button>
                 </div>
             </div>
             <div class="md:col-span-8 bg-gray-50 p-8 md:p-12 flex items-center justify-center relative overflow-hidden">
                 <!-- Content Calendar UI Mockup -->
                 <div class="bg-white shadow-xl rounded-lg w-full h-full border border-gray-200 p-6 relative flex flex-col">
                    <div class="flex gap-2 mb-6 border-b border-gray-100 pb-4">
                        <div class="w-3 h-3 rounded-full bg-red-400"></div>
                        <div class="w-3 h-3 rounded-full bg-yellow-400"></div>
                        <div class="w-3 h-3 rounded-full bg-green-400"></div>
                        <div class="ml-auto flex gap-2">
                            <div class="h-4 w-32 bg-gray-100 rounded-full"></div>
                        </div>
                    </div>
                    
                    <div class="space-y-6">
                        <!-- Header Stats -->
                        <div class="grid grid-cols-4 gap-4">
                             <div class="p-3 bg-gray-50 rounded border border-gray-100">
                                 <div class="text-[10px] text-gray-500 uppercase font-bold">Scheduled</div>
                                 <div class="text-xl font-bold text-gray-900">28</div>
                                 <div class="text-[10px] text-blue-600 font-bold">This month</div>
                             </div>
                             <div class="p-3 bg-gray-50 rounded border border-gray-100">
                                 <div class="text-[10px] text-gray-500 uppercase font-bold">Followers</div>
                                 <div class="text-xl font-bold text-gray-900">1.2k</div>
                                 <div class="text-[10px] text-green-600 font-bold">+127 this week</div>
                             </div>
                             <div class="p-3 bg-gray-50 rounded border border-gray-100">
                                 <div class="text-[10px] text-gray-500 uppercase font-bold">Engagement</div>
                                 <div class="text-xl font-bold text-gray-900">8.4%</div>
                                 <div class="text-[10px] text-green-600 font-bold">+2.1%</div>
                             </div>
                             <div class="p-3 bg-gray-50 rounded border border-gray-100">
                                 <div class="text-[10px] text-gray-500 uppercase font-bold">Time Saved</div>
                                 <div class="text-xl font-bold text-gray-900">12h</div>
                                 <div class="text-[10px] text-gray-400 font-bold">Per week</div>
                             </div>
                        </div>

                        <!-- Content List -->
                        <div class="border border-gray-100 rounded-lg overflow-hidden">
                            <div class="bg-gray-50 px-4 py-2 border-b border-gray-100 flex text-[10px] font-bold text-gray-500 uppercase tracking-wider">
                                <div class="w-2/5">Content</div>
                                <div class="w-1/5">Platform</div>
                                <div class="w-1/5">Date</div>
                                <div class="w-1/5 text-right">Status</div>
                            </div>
                            <div class="divide-y divide-gray-50 text-xs">
                                 {#each [
                                     {content: 'AI agents are transforming...', platform: 'LinkedIn', date: 'Today 9am', status: 'Scheduled', color: 'blue'},
                                     {content: 'Just shipped a new feature...', platform: 'X', date: 'Today 2pm', status: 'Scheduled', color: 'gray'},
                                     {content: 'Thread: How we built V30...', platform: 'X', date: 'Tomorrow', status: 'Ready', color: 'green'},
                                     {content: 'Lessons from 100 users...', platform: 'LinkedIn', date: 'Wed 10am', status: 'Scheduled', color: 'blue'},
                                     {content: 'Why consistency matters...', platform: 'LinkedIn', date: 'Thu 9am', status: 'Scheduled', color: 'blue'}
                                 ] as item}
                                 <div class="px-4 py-3 flex items-center hover:bg-gray-50 transition-colors">
                                     <div class="w-2/5 font-medium text-gray-900 truncate">{item.content}</div>
                                     <div class="w-1/5">
                                         <span class="px-2 py-0.5 rounded text-[10px] font-bold {item.color === 'blue' ? 'bg-blue-100 text-blue-700' : 'bg-gray-100 text-gray-700'}">{item.platform}</span>
                                     </div>
                                     <div class="w-1/5 text-gray-600">{item.date}</div>
                                     <div class="w-1/5 text-right">
                                         <span class="text-[10px] font-bold {item.status === 'Ready' ? 'text-green-600' : 'text-blue-600'}">{item.status}</span>
                                     </div>
                                 </div>
                                 {/each}
                            </div>
                        </div>
                    </div>
                 </div>
             </div>
        </div>
        
        <!-- Bottom Grid of 3 items -->
        <div class="grid md:grid-cols-3 gap-0 mt-0 border-x border-b border-gray-200 divide-x divide-gray-200 bg-white">
            <div class="p-6 flex items-start gap-4 hover:bg-gray-50 transition-colors cursor-pointer">
                <div class="w-6 h-6 rounded-full border border-gray-300 flex-shrink-0 flex items-center justify-center text-xs font-mono">1</div>
                <p class="text-xs text-gray-600 leading-relaxed">V30 analyzes your best content and audience behavior to suggest optimal posting times and topics.</p>
            </div>
            <div class="p-6 flex items-start gap-4 hover:bg-gray-50 transition-colors cursor-pointer">
                <div class="w-6 h-6 rounded-full border border-gray-300 flex-shrink-0 flex items-center justify-center text-xs font-mono">2</div>
                <p class="text-xs text-gray-600 leading-relaxed">Every post is tailored to each platform's unique style and audience expectations for maximum impact.</p>
            </div>
            <div class="p-6 flex items-start gap-4 hover:bg-gray-50 transition-colors cursor-pointer">
                <div class="w-6 h-6 rounded-full border border-gray-300 flex-shrink-0 flex items-center justify-center text-xs font-mono">3</div>
                <p class="text-xs text-gray-600 leading-relaxed">Review and approve posts before they go live, or let V30 auto-publish for complete hands-off automation.</p>
            </div>
        </div>
    </div>
</section>