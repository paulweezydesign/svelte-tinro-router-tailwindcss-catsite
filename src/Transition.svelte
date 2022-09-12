<script>
  import { router } from "tinro";
  import { fade, fly, slide } from "svelte/transition";
  import { cubicIn, elasticOut, linear, quadInOut } from "svelte/easing";
  import { quintOut } from "svelte/easing";
  export let visible;

  function whoosh(node, params) {
    const existingTransform = getComputedStyle(node).transform.replace(
      "none",
      ""
    );

    return {
      delay: params.delay || 2700,
      easing: params.easing || elasticOut,
      css: (t, u) => `transform: ${existingTransform} scale(${t})`,
    };
  }
</script>

{#key $router.path}
  <div
    in:fly={{
      delay: 300,
      duration: 400,
      x: 400,
      y: 200,
      opacity: 0.0,
      easing: cubicIn,
    }}
    out:fade={{ duration: 400, easing: quadInOut }}
  >
    <slot />
  </div>
{/key}
