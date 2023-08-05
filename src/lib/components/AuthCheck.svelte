<script lang="ts">
    import { user } from "$lib/firebase";
</script>

{#if $user}
    <slot />
{:else}
    <h2 class="card-title">You are not logged in</h2>
    <a href="/login" class="text-center text-error">Please sign in to continue</a>
{/if}