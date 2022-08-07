<script lang="ts">
    export let text: string 
</script>

<button class="flex flex-row h-10 w-3/5 justify-center items-center bg-google-white rounded-md shadow-md font-google">
    <img class="w-[18px] mr-[24px]" src="google.svg" alt="Google Icon" />
    {text}
</button>