<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';
	let { children } = $props();
</script>

<svelte:head><link rel="icon" href={favicon} /></svelte:head>


<nav class="flex font-serif items-left px-20 lg:mt-12">
	
	<ul class="flex flexbox gap-6 items-center text-center">
		<li>
			<a href="/about">
				<button class="m-auto p-4 hover:underline"> 
					About
				</button>
			</a>
		</li>
		
		<li>
			<a href="/contact">
				<button class="m-auto p-4 hover:underline "> 
					Contact
				</button>
			</a>
		</li>
	</ul>
	
</nav>

{@render children()}

