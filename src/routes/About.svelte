<section
  class="grid grid-cols-1 items-center justify-center w-[100vw] h-screen  will-change-auto px-4 mx-auto"
>
  <main
    class="container flex item-center flex-col  mx-auto w-screen  max-w-6xl p-4 gap-x-8"
  >
    <h1
      class=" text-6xl md:text-7xl lg:text-8xl xl:text-9xl font-black text-[#242424] mb-8"
    >
      <span
        class="bg-gradient-to-b from-purple-600 to-indigo-700 bg-clip-text text-transparent"
        >About</span
      > us,
    </h1>
    <div
      class="container mx-auto columns-1 md:columns-2 lg:columns-3 max-w-6xl"
    >
      <p class="prose lg:prose-xl">
        This started the way these things always start.. we had lil Pancake(the
        cat) and were happy as can be.. Then one day one of our children brought
        home Bean from her other house and the rest as they say is History.
      </p>
      <p class="">
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. Adipisci,
        quasi fugit. Aspernatur fugit neque, vero quae unde aut ab facere minima
        nisi, placeat officia sint maxime nemo expedita asperiores, dolorem
        atque culpa rem? Accusantium possimus nemo, vitae sapiente nulla
        laboriosam!
      </p>
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. At repellat
        nisi aperiam reiciendis maxime veritatis atque dignissimos quae itaque
        accusamus eius eaque tempora amet recusandae odio, quas minus.
        Reprehenderit, doloremque?
      </p>
    </div>
    <!-- This is a button toggling the modal -->
  </main>
</section>

<style>
  h1 {
    display: grid;
    animation: var(--animation-scale-down) reverse,
      var(--animation-fade-out) reverse;
    animation-timing-function: var(--ease-squish-5);
    animation-duration: 1s;
  }
  .hero {
    line-height: var(--font-lineheight-1);
    font-size: var(--font-size-fluid-3);
    font-weight: var(--font-weight-9);
    font-family: var(--font-sans);
    color: var(--white-0);
  }
</style>
