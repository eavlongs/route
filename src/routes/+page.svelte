<script lang="ts">
	import Contributors from '$lib/components/Index/Contributors.svelte';
	import Features from '$lib/components/Index/Features.svelte';
	import Footer from '$lib/components/Index/Footer.svelte';
	import Hero from '$lib/components/Index/Hero.svelte';
	import Navbar from '$lib/components/Shared/Navbar.svelte';
	import Cta from '$lib/components/Index/CTA.svelte';
	import OurUsers from '$lib/components/Index/OurUsers.svelte';
	import type { PageData } from './$types';

	export let data: PageData;
</script>

<div class="flex flex-col">
	<Navbar />
	<Hero />
	<Features />
	<OurUsers users={data.users} />
	<Cta />
	<Contributors />
	<Footer />
</div>
