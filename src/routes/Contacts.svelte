<div
  class="h-screen  w-screen grid place-items-center bg-gradient-to-b from-purple-600 to-indigo-700 will-change-auto"
>
  <h1 class="text-7xl text-center text-white/90 font-black ">Let's Talk</h1>

  <section class="p-6 w-full  dark:text-coolGray-100">
    <form
      novalidate=""
      class="bg-white container w-full max-w-xl p-8 mx-auto space-y-6 rounded-md shadow dark:bg-coolGray-900 ng-untouched ng-pristine ng-valid"
    >
      <h2 class="w-full text-black/90 text-3xl font-bold leading-tight">
        Contact us
      </h2>
      <div>
        <label for="name" class="block text-white/90 mb-1 ml-1">Name</label>
        <input
          id="name"
          type="text"
          placeholder="Your name"
          required=""
          class=" block w-full p-2 rounded  hover:ring focus:ring hover:border-none border-black border-4 hover:ring-[magenta] focus:ring-[magenta] dark:bg-coolGray-800"
        />
      </div>
      <div>
        <label for="email" class="block  text-white/90 mb-1 ml-1">Email</label>
        <input
          id="email"
          type="email"
          placeholder="Your email"
          required=""
          class="block w-full p-2 rounded focus:outline-none  hover:ring hover:bg-none focus:ring hover:border-none border-black border-4 hover:ring-[magenta] focus:ring-[magenta] dark:bg-coolGray-800"
        />
      </div>
      <div>
        <label for="message" class="block  text-white/90 mb-1 ml-1"
          >Message</label
        >
        <textarea
          id="message"
          type="text"
          placeholder="Message..."
          class="block w-full p-2 hover:bg-none rounded autoexpand focus:outline-none  hover:ring focus:ring hover:border-none border-black border-4 hover:ring-[magenta] focus:ring-[magenta]  dark:bg-coolGray-800"
        />
      </div>
      <div>
        <button
          type="submit"
          class="bg-black w-full px-4 py-3 font-light tracking-wide text-white rounded shadow-lg shadow-indigo-700/40 focus:outline-none focus:ring hover:ring focus:ring-opacity-50 dark:bg-[magenta]focus:ring-[magenta] hover:ring-[magenta] dark:text-coolGray-900"
          >Send</button
        >
      </div>
    </form>
  </section>
</div>

<style>
  .card {
    border-radius: var(--radius-2);
    background-color: var(--gray-0);
    color: black;
    padding: var(--size-fluid-3);
    box-shadow: var(--shadow-2);
  }

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
