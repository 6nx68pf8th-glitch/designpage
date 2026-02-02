<script lang="ts">
    import logo from '$lib/assets/logo.svg'

    let menuOpen = false;
    let blur = 'none';
    let gray = 100;

    function menu() {
        menuOpen = !menuOpen;
        
        if(menuOpen){
            blur = 'sm';
            gray = 0;
        }
        else if(!menuOpen){
            blur = 'none';
            gray = 100;
        }
        


    }
    
    
</script>

<section class="font-serif mt-12 mb-24 my-10">
    <div class="justify-center items-center text-center">
       
        <button onclick={menu}>
            <img 
                src={logo} 
                alt="" 
                class="w-full" 
            >
        </button>
        {#if menuOpen}
        <div class="flex justify-center items-center text-center">
            <ul>
                <li><a href="/about">About</a></li>
                <li><a href="/contact">Contact</a></li>
            </ul>
        </div>
        {/if}
    </div>

    
</section>
