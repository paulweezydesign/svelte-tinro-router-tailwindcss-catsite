<script>
  export let address;
  export let description;
  export let name;
</script>

<div
  class="relative shadow-lg rounded-b-[15px] shadow-black-40 hover:shadow-xl hover:shadow-black/60 w-[200px]  hover:scale-105 will-change transform-all"
>
  <div
    class="absolute rounded-b-[15px] bottom-0 overflow-auto w-[200px]  px-2 pb-2 text-shadow text-white bg-gradient-to-b from-transparent to-black/80"
  >
    <h1 class=" text-center font-bold text-2xl text-white mx-auto">{name}</h1>
    <p class="prose text-sm text-white">{description}</p>
  </div>
  <img class="rounded-[15px]" src={address} alt="pic" />
</div>
