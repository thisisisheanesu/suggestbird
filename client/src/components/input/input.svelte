<script lang="ts">
    import type { InputTypeProps } from "./input.types";
    export let type: InputTypeProps
    export let name: string
    export let autocomplete: string = ""     
    export let id: string = name
    export let placeholder: string = name[0].toUpperCase() + name.slice(1).toLowerCase()
    export let className: string = "h-10 w-full mb-4 text-gray-400 p-4 bg-gray-100 focus:outline-none rounded"
</script>

<input 
    id={id}
    type={type}
    name={name}
    autocomplete={autocomplete}
    placeholder={placeholder}
    class={className} />
    