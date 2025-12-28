<div class="w-full">
  <div
    class="bg-[#F5F5F5] rounded-2xl p-4 md:p-8 font-mono leading-relaxed border-4 sm:border-6 border-white"
  >
    <div class="flex overflow-x-auto sm:text-[8px] md:text-base">
      <div
        class="text-blue-400 pr-3 sm:pr-4 md:pr-6 select-none text-right shrink-0"
        style="min-width: 30px;"
      >
        {#each Array(16) as _, i}
          <div class="leading-relaxed">{i + 1}</div>
        {/each}
      </div>

      <div class="flex-1 min-w-0 text-gray-800">
        <div class="leading-relaxed whitespace-nowrap">
          <span class="text-purple-600">const</span>
          <span class="text-gray-800">Chainpaye</span>
          = <span class="text-purple-600">new</span>
          <span class="text-blue-500">ChainpayeWidget</span>({"{"})
        </div>
        <div class="leading-relaxed pl-4 sm:pl-6 whitespace-nowrap">
          <span class="text-orange-500">env</span>:
          <span class="text-green-600">"production"</span>,
        </div>
        <div class="leading-relaxed pl-4 sm:pl-6 whitespace-nowrap">
          <span class="text-orange-500">action</span>:
          <span class="text-green-600">"send_payment"</span>,
        </div>
        <div class="leading-relaxed pl-4 sm:pl-6 whitespace-nowrap">
          <span class="text-orange-500">fromCurrency</span>:
          <span class="text-green-600">"USD"</span>,
        </div>
        <div class="leading-relaxed pl-4 sm:pl-6 whitespace-nowrap">
          <span class="text-orange-500">toCurrency</span>:
          <span class="text-green-600">"NGN"</span>,
        </div>
        <div class="leading-relaxed pl-4 sm:pl-6 whitespace-nowrap">
          <span class="text-orange-500">apiKey</span>:
          <span class="text-green-600">"ck_live_89f1JKS0xPqA90217x"</span>,
        </div>
        <div class="leading-relaxed whitespace-nowrap">{"}"},</div>
        <div class="leading-relaxed pl-4 sm:pl-6 whitespace-nowrap">
          <span class="text-orange-500">callback</span>: {"{"}
        </div>
        <div class="leading-relaxed pl-8 sm:pl-12 whitespace-nowrap">
          <span class="text-orange-500">onStatus</span>: (<span
            class="text-gray-800">status</span
          >) => {"{"}
        </div>
        <div class="leading-relaxed pl-12 sm:pl-20 whitespace-nowrap">
          <span class="text-gray-800">console</span>.<span
            class="text-purple-600">log</span
          >(<span class="text-green-600">"Payment status:"</span>,
          <span class="text-gray-800">status</span>);
        </div>
        <div class="leading-relaxed pl-8 sm:pl-12 whitespace-nowrap">{"}"}</div>
        <div class="leading-relaxed pl-4 sm:pl-6 whitespace-nowrap">{"}"}</div>
        <div class="leading-relaxed whitespace-nowrap">{"}"});</div>
        <div class="leading-relaxed whitespace-nowrap">&nbsp;</div>
        <div class="leading-relaxed whitespace-nowrap">
          <span class="text-gray-800">Chainpaye</span>.<span
            class="text-blue-500">open</span
          >();
        </div>
      </div>
    </div>
  </div>
</div>
