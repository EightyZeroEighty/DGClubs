<script>
	import '../app.css';
	let { children } = $props();
	import { slide } from 'svelte/transition'; // Add this import
	import { onMount } from 'svelte';

	// State
	let isMobileMenuOpen = $state(false);
	let isScrolled = $state(false);

	// Navigation data
	const productLinks = [
		{ href: '/features', label: 'Features' },
		{ href: '/pricing', label: 'Pricing' },
		{ href: '/integrations', label: 'Integrations' }
	];

	const resourceLinks = [
		{ href: '/blog', label: 'Blog' },
		{ href: '/guides', label: 'Guides' },
		{ href: '/case-studies', label: 'Case Studies' },
		{ href: '/webinars', label: 'Webinars' }
	];

	const supportLinks = [
		{ href: '/help', label: 'Help Center' },
		{ href: '/documentation', label: 'Documentation' },
		{ href: '/faq', label: 'FAQ' },
		{ href: '/contact', label: 'Contact Us' }
	];

	// Handle scroll events
	onMount(() => {
		const handleScroll = () => {
			isScrolled = window.scrollY > 10;
		};

		window.addEventListener('scroll', handleScroll);
		return () => window.removeEventListener('scroll', handleScroll);
	});

	// Toggle mobile menu
	function toggleMobileMenu() {
		isMobileMenuOpen = !isMobileMenuOpen;
	}
</script>

<nav class="sticky top-0 z-50 bg-white {isScrolled ? 'shadow-lg' : ''}">
	<div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
		<div class="flex h-16 justify-between">
			<!-- Logo and Brand -->
			<div class="flex items-center">
				<a href="/" class="flex items-center">
					<span class="text-2xl font-bold text-blue-600">DGClubs</span>
				</a>
			</div>

			<!-- Desktop Navigation -->
			<div class="hidden items-center space-x-1 md:flex">
				<!-- Products Dropdown -->
				<div class="group relative">
					<button class="flex items-center px-3 py-2 text-gray-600 hover:text-blue-600">
						Product
						<svg class="ml-1 h-4 w-4" fill="none" stroke="currentColor" viewBox="0 0 24 24">
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M19 9l-7 7-7-7"
							/>
						</svg>
					</button>
					<div
						class="invisible absolute left-0 mt-2 w-48 rounded-md bg-white opacity-0 shadow-lg transition-all duration-200 group-hover:visible group-hover:opacity-100"
					>
						{#each productLinks as { href, label }}
							<a {href} class="block px-4 py-2 text-sm text-gray-700 hover:bg-blue-50">
								{label}
							</a>
						{/each}
					</div>
				</div>

				<!-- Resources Dropdown -->
				<div class="group relative">
					<button class="flex items-center px-3 py-2 text-gray-600 hover:text-blue-600">
						Resources
						<svg class="ml-1 h-4 w-4" fill="none" stroke="currentColor" viewBox="0 0 24 24">
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M19 9l-7 7-7-7"
							/>
						</svg>
					</button>
					<div
						class="invisible absolute left-0 mt-2 w-48 rounded-md bg-white opacity-0 shadow-lg transition-all duration-200 group-hover:visible group-hover:opacity-100"
					>
						{#each resourceLinks as { href, label }}
							<a {href} class="block px-4 py-2 text-sm text-gray-700 hover:bg-blue-50">
								{label}
							</a>
						{/each}
					</div>
				</div>

				<a href="/about" class="px-3 py-2 text-gray-600 hover:text-blue-600">About</a>

				<!-- Support Dropdown -->
				<div class="group relative">
					<button class="flex items-center px-3 py-2 text-gray-600 hover:text-blue-600">
						Support
						<svg class="ml-1 h-4 w-4" fill="none" stroke="currentColor" viewBox="0 0 24 24">
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M19 9l-7 7-7-7"
							/>
						</svg>
					</button>
					<div
						class="invisible absolute left-0 mt-2 w-48 rounded-md bg-white opacity-0 shadow-lg transition-all duration-200 group-hover:visible group-hover:opacity-100"
					>
						{#each supportLinks as { href, label }}
							<a {href} class="block px-4 py-2 text-sm text-gray-700 hover:bg-blue-50">
								{label}
							</a>
						{/each}
					</div>
				</div>
			</div>

			<!-- Right Side - Auth Buttons -->
			<div class="hidden items-center space-x-4 md:flex">
				<a href="/login" class="text-gray-600 hover:text-blue-600">Login</a>
				<a href="/signup" class="rounded-lg bg-blue-600 px-4 py-2 text-white hover:bg-blue-700">
					Start Free Trial
				</a>
			</div>

			<!-- Mobile Menu Button -->
			<div class="flex items-center md:hidden">
				<button
					onclick={toggleMobileMenu}
					class="rounded-md p-2 hover:bg-gray-100 focus:outline-none"
					aria-label="Toggle mobile menu"
				>
					<svg class="h-6 w-6 text-gray-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
						<path
							stroke-linecap="round"
							stroke-linejoin="round"
							stroke-width="2"
							d="M4 6h16M4 12h16M4 18h16"
						/>
					</svg>
				</button>
			</div>
		</div>
	</div>

	<!-- Mobile Menu -->
	{#if isMobileMenuOpen}
		<div class="md:hidden" transition:slide={{ duration: 200 }}>
			<div class="space-y-1 px-2 pb-3 pt-2">
				{#each productLinks as { href, label }}
					<a {href} class="block px-3 py-2 text-base font-medium text-gray-600 hover:bg-gray-50">
						{label}
					</a>
				{/each}

				{#each resourceLinks as { href, label }}
					<a {href} class="block px-3 py-2 text-base font-medium text-gray-600 hover:bg-gray-50">
						{label}
					</a>
				{/each}

				<a
					href="/about"
					class="block px-3 py-2 text-base font-medium text-gray-600 hover:bg-gray-50"
				>
					About
				</a>

				{#each supportLinks as { href, label }}
					<a {href} class="block px-3 py-2 text-base font-medium text-gray-600 hover:bg-gray-50">
						{label}
					</a>
				{/each}

				<div class="border-t border-gray-200 pb-3 pt-4">
					<a
						href="/login"
						class="block px-3 py-2 text-base font-medium text-gray-600 hover:bg-gray-50"
					>
						Login
					</a>
					<a
						href="/signup"
						class="block px-3 py-2 text-base font-medium text-blue-600 hover:bg-gray-50"
					>
						Start Free Trial
					</a>
				</div>
			</div>
		</div>
	{/if}
</nav>
<div class="bg-gray-50 font-sans">
	{@render children()}
</div>
<!-- Footer -->
<footer class="bg-gray-800 text-white">
	<div class="mx-auto max-w-7xl px-4 py-12 sm:px-6 lg:px-8">
		<div class="grid gap-8 md:grid-cols-4">
			<div>
				<h3 class="mb-4 text-2xl font-bold">DGClubs</h3>
				<p class="text-gray-400">Making disc golf club management simple and efficient.</p>
			</div>
			<div>
				<h4 class="mb-4 font-semibold">Product</h4>
				<ul class="space-y-2 text-gray-400">
					<li><a href="#features" class="hover:text-white">Features</a></li>
					<li><a href="#pricing" class="hover:text-white">Pricing</a></li>
					<li><a href="#demo" class="hover:text-white">Request Demo</a></li>
				</ul>
			</div>
			<div>
				<h4 class="mb-4 font-semibold">Company</h4>
				<ul class="space-y-2 text-gray-400">
					<li><a href="#about" class="hover:text-white">About</a></li>
					<li><a href="#contact" class="hover:text-white">Contact</a></li>
					<li><a href="#privacy" class="hover:text-white">Privacy Policy</a></li>
				</ul>
			</div>
			<div>
				<h4 class="mb-4 font-semibold">Connect</h4>
				<ul class="space-y-2 text-gray-400">
					<li><a href="#twitter" class="hover:text-white">Twitter</a></li>
					<li><a href="#facebook" class="hover:text-white">Facebook</a></li>
					<li><a href="#linkedin" class="hover:text-white">LinkedIn</a></li>
				</ul>
			</div>
		</div>
		<div class="mt-8 border-t border-gray-700 pt-8 text-center text-gray-400">
			<p>&copy; 2024 DGClubs. All rights reserved.</p>
		</div>
	</div>
</footer>

