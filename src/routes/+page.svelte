<script lang="ts">
  const monkeyCount = 8;
  console.log(Array.from({ length: monkeyCount }))
</script>

<div class="w-full grid grid-cols-5 bg-[url(/img/diamond.jpg)] bg-repeat bg-200 min-h-screen">
  <div class="h-full col-span-1 bg-[url(/img/pickaxe.gif)] bg-repeat-y bg-contain"></div>
  <main class="col-span-3 max-w-4xl mx-auto">
    <!-- Header -->
    <div class="flex flex-col max-w-xl px-4 mx-auto justify-center text-center header-text text-white bg-[url(/img/buff_mark.jpg)] bg-contain aspect-[754/960]">
      <h1 class="text-6xl sm:text-8xl pt-8 sm:pt-32">
        Cuck SMP©
      </h1>
      <h2 class="text-3xl mt-8">
        In Cuck We Trust
      </h2>
    </div>

    <!-- Join the discord link -->
    <div class="w-full mx-auto flex max-w-xl">
      <a href="https://discord.gg/PJEPxakEFc" class="mt-8 mx-auto">
        <img src="img/join-the-discord.gif" alt="Join the discord" class=" box-border hover:outline-dashed outline-red-600 transition-all">
      </a>
    </div>

    <!-- Meet the monkey -->
    <div>
      <h2 class="text-center text-4xl sm:text-5xl md:text-7xl mt-8 md:-mb-20 meet-the font-thin relative">Meet The</h2>
      <img src="img/moneky.gif" alt="Monkey">
    </div>

    <!-- Monkey GIFS -->
    <div class="grid grid-cols-1 md:grid-cols-2 mt-16 space-y-4">
      {#each Array.from({ length: monkeyCount }) as _, i (i)}
        <div class="flex">
          <a href="http://sciencekids.co.nz/sciencefacts/animals/monkey.html" class="m-auto">
            <img src="img/mokey/{i+1}.gif" alt="">
          </a>
        </div>
      {/each}
    </div>

    <!-- FAQ -->
    <div class="flex flex-col mx-auto mt-8">
      <h2 class="header-text text-center text-8xl text-black font-thin mb-24">
        FAQ''s
      </h2>

      <div class="grid grid-cols-1 sm:grid-cols-2">
        <img src="img/john-wick.gif" alt="Thanos Fortnite wow" class="w-4/5">
        <img src="img/swim.gif" alt="No idea what this is" class="w-4/5">
      </div>

      <div>
        <p class="text-center py-4 text-sm sm:text-base">
          Disclaimer: dont even think about making fun of me. I am more powerful than any of you could imagine. Watch your fucking step when you enter here swine.
        </p>
      </div>
    </div>
  </main>
  <div class="h-full col-span-1 bg-[url(/img/pickaxe.gif)] bg-repeat-y bg-contain"></div>
</div>

<style lang="postcss">
  .header-text {
    text-shadow: 2px 2px red;
  }

  .bg-200 {
    background-size: 200px;
  }

  .meet-the {
    text-shadow: 6px 6px #ed8421;
    @apply z-10 text-gray-800;
  }
</style>