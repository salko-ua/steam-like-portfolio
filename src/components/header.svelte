<script>
  import { asset } from "$app/paths";
  import { portfolioData } from "$lib/data";
</script>

<div
  class="
    flex
    max-xs:h-fit
    h-50 w-full p-2
    lg:col-span-2
  "
>
  <!-- avatar -->
  <div
    class="
    min-h-42 min-w-42 h-42 w-42
    max-xs:min-h-24 max-xs:min-w-24 max-xs:h-24 max-xs:w-24
    mr-4
    [clip-path:polygon(0%_15%,_10%_5%,_20%_12%,_30%_3%,_40%_15%,_50%_4%,_60%_12%,_70%_2%,_85%_14%,_100%_8%,_100%_85%,_90%_95%,_80%_88%,_70%_98%,_60%_85%,_50%_95%,_40%_88%,_30%_100%,_15%_85%,_0%_92%)]
  "
  >
    <img
      alt="portrayal"
      src={asset("/pfp.jpg")}
      class="size-full object-cover"
    />
  </div>
  <!-- name -->
  <div class="flex flex-col lg:pl-4 lg:pt-2">
    <div class="text-white font-light text-2xl mb-2">SALO</div>
    <div class="text-gray-300 text-xs mb-4 ml-2">
      {portfolioData.header.location}
    </div>
    <div class="text-gray-300 text-xs">{portfolioData.header.profession}</div>
    <div class="text-gray-100 text-xs">
      <a href={portfolioData.header.githubLink}>GitHub link</a>
    </div>
  </div>
</div>
