<script>
  import KittenCard from "/src/components/KittenCard.svelte";
  import { fade } from "svelte/transition";
  import { onMount } from "svelte";
  let selection;

  function setSelection(res) {
    selection = res;
  }
  let show = true;
  onMount(() => {
    show = true;
  });
  let cats = [
    {
      id: "1",
      name: "Filaberta",
      description:
        "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Et, iure, odit laboriosam sunt quibusdam optio autem nobis dolor esse tenetur.",
      route: "/Filaberta",
      address: "http://placekitten.com/g/200/350",
    },
    {
      id: "2",
      name: "Garfield",
      description:
        "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Et, iure, odit laboriosam sunt quibusdam optio autem nobis dolor esse tenetur.",
      route: "/Garfield",
      address: "http://placekitten.com/g/200/350",
    },
    {
      id: "3",
      name: "Pancake",
      description:
        "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Et, iure, odit laboriosam sunt quibusdam optio autem nobis dolor esse tenetur.",
      route: "/Pancake",
      address: "http://placekitten.com/g/200/350",
    },
    {
      id: "4",
      name: "Fluffy",
      description:
        "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Et, iure, odit laboriosam sunt quibusdam optio autem nobis dolor esse tenetur.",
      route: "/Fluffy",
      address: "http://placekitten.com/g/200/350",
    },
    {
      id: "5",
      name: "Baby Bean",
      description:
        "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Et, iure, odit laboriosam sunt quibusdam optio autem nobis dolor esse tenetur.",
      route: "/BabyBean",
      address: "http://placekitten.com/g/200/350",
    },
    {
      id: "6",
      name: "Baby Bean II",
      description:
        "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Et, iure, odit laboriosam sunt quibusdam optio autem nobis dolor esse tenetur.",
      route: "BabyBeanjr",
      address: "http://placekitten.com/g/200/350",
    },
    {
      id: "7",
      name: "Little Baby Sunshine",
      description:
        "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Et, iure, odit laboriosam sunt quibusdam optio autem nobis dolor esse tenetur.",
      route: "/BabySunshine",
      address: "http://placekitten.com/g/200/350",
    },
    {
      id: "8",
      name: "Fat head",
      description:
        "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Et, iure, odit laboriosam sunt quibusdam optio autem nobis dolor esse tenetur.",
      route: "/FatHead",
      address: "http://placekitten.com/g/200/350",
    },
    {
      id: "9",
      name: "Bean",
      description:
        "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Et, iure, odit laboriosam sunt quibusdam optio autem nobis dolor esse tenetur.",
      route: "/Bean",
      address: "http://placekitten.com/g/200/350",
    },
    {
      id: "10",
      name: "Rocket",
      description:
        "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Et, iure, odit laboriosam sunt quibusdam optio autem nobis dolor esse tenetur.",
      route: "/Rocket",
      address: "http://placekitten.com/g/200/350",
    },
    {
      id: "11",
      name: "Angel",
      description:
        "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Et, iure, odit laboriosam sunt quibusdam optio autem nobis dolor esse tenetur.",
      route: "/Angel",
      address: "http://placekitten.com/g/200/350",
    },
    {
      id: "12",
      name: "Mean kitty",
      description:
        "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Et, iure, odit laboriosam sunt quibusdam optio autem nobis dolor esse tenetur.",
      route: "/MeanKitty",
      address: "http://placekitten.com/g/200/350",
    },
    {
      id: "13",
      name: "Nice kitty",
      description:
        "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Et, iure, odit laboriosam sunt quibusdam optio autem nobis dolor esse tenetur.",
      route: "/NiceKitty",
      address: "http://placekitten.com/g/200/350",
    },
  ];
</script>

<section class="">
  <h1 class="text-7xl font-black text-center my-[50px] ">
    Let the <span
      class="bg-gradient-to-b from-purple-600 to-indigo-700 bg-clip-text text-transparent"
      >cuteness</span
    > begin....
  </h1>

  <div class="flex item-center justify-center">
    {#if show}
      <section class="kitten-grid   ">
        {#each cats as cat (cat.id)}
          <a href={cat.route}>
            <KittenCard
              class=""
              name={cat.name}
              description={cat.description}
              address={cat.address}
            />
          </a>
        {/each}
      </section>
    {/if}
  </div>
</section>

<style type="text/css">
  .kitten-grid {
    display: grid;
    max-width: 80vw;
    grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
    grid-gap: 1.5rem;
    color: #fff;
    margin-right: auto;
    margin-left: auto;
  }
  hover:a {
    color: deeppink;
  }
</style>
