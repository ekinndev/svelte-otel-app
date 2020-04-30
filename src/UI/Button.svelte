<script>
  export let type = "button";
  export let href = null;
  export let lightOrDark = false;
  export let disabled = false;
  import { link } from "svelte-routing";

</script>

<style>
  .btn {
    display: inline-block;
    font-size: 18px;
    color: #fff;
    background: #333;
    padding: 13px 20px;
    border: none;
    border-radius: 8px;
    cursor: pointer;
  }
  .btn:hover {
    background: #f7c08a;
    color: #333;
  }
  .btn-light {
    background: #f4f4f4;
    color: #333;
  }
</style>

{#if href}
  <a class="btn" use:link class:btn-light="{lightOrDark}" {href}>
    <slot />
  </a>
{:else}
  <button class="btn" use:link {type} class:btn-light="{lightOrDark}" on:click {disabled}>
    <slot />
  </button>
{/if}
