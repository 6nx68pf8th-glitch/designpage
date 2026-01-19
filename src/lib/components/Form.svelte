<script lang="ts">
    let formShow = false

    function click() {
        formShow = !formShow;   
    }
</script>

<div class="mt-4">
    {#if !formShow}
    <button onclick={click} class="text-blue-700 xl:text-xl xl:bg-slate-700/0 bg-slate-700 xl:p-0 p-2 rounded xl:hover:underline">
        Contact Form
    </button>
    {:else}
    <form action="" class="mx-20 py-6">
        <section class="m-3">
            <input 
                type="text" 
                name="name" 
                id="name" 
                placeholder="Name" 
                required 
                class="rounded border-0 m-1 bg-blue-100"
            >
            
            <input 
                type="text" 
                name="email" 
                id="email" 
                placeholder="Email" 
                required 
                class="rounded border-0 m-1 bg-blue-100"
            >
        </section>
       
        <section class="m-3">
            <textarea 
                name="message" 
                id="message" 
               
                placeholder="Your mesage here: " 
                class="rounded bg-blue-100 border-0 w-auto m-1"
            ></textarea>
        </section>
        
        <section class="m-6 text-center">
             <input type="submit" class="button hover:underline px-2">
            <button onclick={click} class=" hover:underline px-2 ">Cancel</button>
        </section>
        
       
    </form>
    {/if}
</div>

<style>

</style>