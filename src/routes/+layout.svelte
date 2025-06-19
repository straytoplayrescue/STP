<script lang="ts">
  import { injectAnalytics } from '@vercel/analytics/sveltekit';
  // Initialize analytics on the client
  injectAnalytics();

</script>

<header>
  <h1>Stray To Play Rescue</h1>
Save the dogs!!!
</header>

<slot />

<footer>
  © {new Date().getFullYear()} Stray To Play Rescue
</footer>