<script lang="ts">
    import GoogleButton from "./google.svelte"

    export let text: string
    export let isThirdParty: boolean = false
</script>

{#if isThirdParty}
<GoogleButton text={text} />
{:else}
<button class="h-10 w-3/5 mb-4 bg-primary-700 font-bold text-white rounded-md shadow-md hover:bg-primary-600">
    {text}
</button>
{/if}