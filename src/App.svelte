<script>
  import { Route, active } from "tinro";
  import Contacts from "/src/routes/Contacts.svelte"; // <h1>Contacts</h1>
  import About from "/src/routes/About.svelte";
  import Kittens from "/src/routes/Kittens.svelte";
  import Transition from "./Transition.svelte";
  import Home from "/src/routes/Home.svelte";
  import Filaberta from "/src/routes/Filaberta.svelte";
  import Pancake from "/src/routes/Pancake.svelte";
  import Garfield from "/src/routes/Garfield.svelte";
  import BabyBean from "/src/routes/BabyBean.svelte";
  import Fluffy from "/src/routes/Fluffy.svelte";
  import BabyBeanjr from "/src/routes/BabyBeanjr.svelte";
  import Rocket from "/src/routes/Rocket.svelte";
  import BabySunshine from "/src/routes/BabySunshine.svelte";
  import FatHead from "/src/routes/FatHead.svelte";
  import MeanKitty from "/src/routes/MeanKitty.svelte";
  import NiceKitty from "/src/routes/NiceKitty.svelte";
</script>

<nav
  class="grid grid-cols-1 md:grid-cols-2 items-center px-[6%] w-[100vw] shadow-lg shadow-black-40 py-4"
>
  <div class="">
    <a href="/" class="">
      <h1 class="text-xl font-black mx-auto">My Cute Kittens</h1>
    </a>
  </div>
  <div class="flex justify-center  md:justify-end">
    <a
      class="mr-8 hover:text-[deeppink] active:text-[deeppink]"
      href="/"
      use:active>Home</a
    >
    <a class="mr-8" href="/about">About</a>
    <a class="mr-8" href="/kittens">Kittens</a>
    <a class="" href="/contacts">Contacts</a>
  </div>
  <div class="" />
</nav>
<Transition class="will-change-auto">
  <Route path="/"><Home /></Route>
  <Route path="/about"><About /></Route>
  <Route path="/kittens">
    <Kittens />
  </Route>
  <Route path="/contacts"><Contacts /></Route>
  <Route path="/Filaberta"><Filaberta /></Route>
  <Route path="/Pancake"><Pancake /></Route>
  <Route path="/Garfield"><Garfield /></Route>
  <Route path="/Fluffy"><Fluffy /></Route>
  <Route path="/BabyBean"><BabyBean /></Route>
  <Route path="/BabyBeanjr"><BabyBeanjr /></Route>
  <Route path="/BabySunshine"><BabySunshine /></Route>
  <Route path="/FatHead"><FatHead /></Route>
  <Route path="/Bean"><Bean /></Route>
  <Route path="/Angel"><Angel /></Route>
  <Route path="/Rocket"><Rocket /></Route>
  <Route path="/MeanKitty"><MeanKitty /></Route>
  <Route path="/NiceKitty"><NiceKitty /></Route>
</Transition>

<style type="text/css">
  :active a {
    color: deeppink;
  }

  :hover a {
    color: deeppink;
  }
</style>
