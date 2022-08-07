<script lang="ts">
    import type { InputTypeProps } from "./input.types";
    export let type: InputTypeProps
    export let name: string
    export let autocomplete: string = ""     
    export let id: string = name
    export let placeholder: string = name[0].toUpperCase() + name.slice(1).toLowerCase()
    export let className: string = "h-10 w-full mb-4 text-gray-400 p-4 border-b-2 border-b-gray-300 focus:border-primary-600 focus:outline-none"
</script>

<input 
    id={id}
    type={type}
    name={name}
    autocomplete={autocomplete}
    placeholder={placeholder}
    class={className} />
    