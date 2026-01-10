<script>
    import Form from "$lib/components/Form.svelte";
</script>


<section class="flex font-serif">
    <div class="w-1/3 m-20 justify-center text-center text-xl">
        <h2 class="font-bold m-5 text-left">
            Stack 🔗
        </h2>

        <ul class="text-left ml-10">
            <li><a href="https://svelte.dev">Svelte</a></li>
            <li><a href="https://www.typescriptlang.org">TypeScript</a></li>
            <li><a href="https://nodejs.org">Node.js</a></li>
            <li><a href="https://www.python.org">Python</a></li>
        </ul>
       
        <h2 class="font-bold m-5 text-left">
            Skills
        </h2>

        <ul class="text-left ml-10">
            <li>UX Design</li>
            <li>Visual Design</li>
            <li>Prototyping</li>
        </ul>
    </div>

    <div class="w-2/3 justify-center items-center text-center m-20">
        <h1 class=" text-xl items-center text-center font-bold m-5">
            Let's Chat
        </h1>
        <p class="text-left m-6">
            From visualizing concepts to user research, individualized approaches propel you on the journey to success! If you have an idea you would like to make happen, reach out to talk about how to get the results you’re looking for. 
        </p>

        <div class="text-left m-6">
            <Form /> 
        </div>
    </div>
</section>

<section>
    <figure class="flex flex-col gap-1 overflow-auto py-5 mt-12 mb-24 scroll-auto">
        <div class="not-prose rounded-lg snap-x">
                <div class="flex  snap-start overflow-x-scroll scroll-ml-2 gap-2 rounded-3xl inset-ring inset-ring-gray-800/20">
                    
                </div>
        
        </div>


    </figure>
</section>

<style>
    a:hover {
        text-decoration: underline;
    }
</style>