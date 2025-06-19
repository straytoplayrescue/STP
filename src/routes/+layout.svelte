<script lang="ts">
  import { injectAnalytics } from '@vercel/analytics/sveltekit';
  // Initialize analytics on the client
  injectAnalytics();

  export let data: { user: any; path: string };
</script>

<header>
  <h1>Stray To Play Rescue</h1>
  {#if data.user}
    <nav>Welcome, {data.user.username}</nav>
  {:else}
    <nav><a href="/login">Log in</a></nav>
  {/if}
</header>

<slot />

<footer>
  © {new Date().getFullYear()} Stray To Play Rescue
</footer>