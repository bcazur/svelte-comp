<script lang="ts">
import { onMount } from "svelte";


    let time: string;
    export let name: string = "unknown";

    onMount(()=>{
        time = new Date().toISOString();
    });
</script>

<div class="placeholder-component">
    <p>Hello {name}. The time is: {time}</p>
</div>

<style>
    .placeholder-component{
        padding: 1rem;
        border: 1px solid black;
    }
</style>