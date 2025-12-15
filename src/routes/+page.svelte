<script lang="ts">
	import { onMount } from 'svelte';

	let scrollY = 0;
</script>

<svelte:window bind:scrollY />

<div class="font-sans text-gray-900 antialiased selection:bg-primary-100 selection:text-primary-900">
	<!-- Header -->
	<header class="fixed top-0 left-0 right-0 z-40 bg-white/80 backdrop-blur-md border-b border-gray-100">
		<div class="px-6 md:px-12 lg:px-24 py-4 flex items-center justify-between">
			<div class="flex items-center gap-2">
				<svg class="w-8 h-8 text-gray-900" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
					<path
						fill-rule="evenodd"
						clip-rule="evenodd"
						d="M5.0473 17.8386L5.69453 18.9586V18.9601H18.3003L18.9314 17.84H6.34063L6.82626 16.9993H19.4308L20.078 15.8807H7.47237L7.95715 15.0414H16.0358L16.0366 15.0429L16.0375 15.0414H20.5603L20.5612 15.0429L21.2084 13.9228L21.208 13.922L21.2084 13.9213H21.2075L14.9084 3.00677L14.9106 3.00296L14.9062 3.00296L13.6177 3.00296L5.0473 17.8386ZM14.261 4.12767L13.7751 4.96887L18.9438 13.9213H19.9139L14.261 4.12767ZM13.1286 6.08808L12.6467 6.9225L16.6749 13.9006L16.6634 13.9213H17.6511L13.1286 6.08808ZM11.9999 8.04225L8.60411 13.9213H15.3899L11.9999 8.04225ZM6.99833 3.30006C7.33866 3.10343 7.7248 2.99993 8.11786 3L2.30033 13.0776C2.10357 12.7371 2 12.3508 2 11.9575C2 11.5643 2.10357 11.178 2.30033 10.8375L6.17916 4.12006C6.37543 3.77951 6.65798 3.49669 6.99833 3.30006ZM9.08869 3H10.3816L3.43223 15.0384L2.785 13.9184L9.08869 3ZM11.3509 3H12.6424L4.56262 16.9963L3.91691 15.8777L11.3509 3ZM21.7064 13.0598C21.8988 12.7254 22 12.3463 22 11.9605C22 11.5746 21.8988 11.1956 21.7064 10.8611L17.8039 4.10233C17.6108 3.7681 17.3331 3.49057 16.9987 3.2976C16.6644 3.10463 16.2852 3.00302 15.8992 3.00296H15.8741L21.6931 13.082L21.7064 13.0598ZM17.7995 19.7994H6.17916C6.37472 20.1412 6.65692 20.4253 6.99728 20.6232C7.33763 20.8212 7.72414 20.9258 8.11786 20.9269H15.8829C16.2737 20.9261 16.6572 20.8212 16.994 20.6231C17.3309 20.4249 17.6089 20.1406 17.7995 19.7994Z"
						fill="currentColor"
					/>
				</svg>
				<span class="font-semibold text-xl">Eightyfour Commerce</span>
			</div>
			<nav class="hidden md:flex items-center gap-8">
				<a href="#services" class="text-sm text-gray-600 hover:text-gray-900 transition-colors">Services</a>
				<a href="#process" class="text-sm text-gray-600 hover:text-gray-900 transition-colors">Process</a>
				<a href="#results" class="text-sm text-gray-600 hover:text-gray-900 transition-colors">Results</a>
				<a href="#contact" class="text-sm bg-gray-900 text-white px-4 py-2 rounded-lg hover:bg-gray-800 transition-colors">Get Started</a>
			</nav>
		</div>
	</header>

	<!-- Hero Section -->
	<section class="relative min-h-screen w-full bg-white text-gray-900 px-6 md:px-12 lg:px-24 pt-32 pb-24 flex flex-col justify-center">
		<div class="max-w-6xl">
			<div class="inline-block px-4 py-2 bg-primary-50 text-primary-700 rounded-full text-sm font-medium mb-8">
				20+ Years of E-commerce Expertise
			</div>
			<h1 class="font-serif text-5xl md:text-7xl lg:text-8xl leading-[1.1] md:leading-[1.1] tracking-tight mb-8">
				Drive profitable growth with expert platform management
			</h1>
			<p class="text-xl md:text-2xl text-gray-600 max-w-3xl leading-relaxed mb-12">
				We specialize in helping brands scale through strategic platform management and hands-on execution. Focus on building your brand while we handle strategy, operations, and optimization.
			</p>
			<div class="flex flex-col sm:flex-row gap-4">
				<a href="#contact" class="inline-flex items-center justify-center px-8 py-4 bg-gray-900 text-white rounded-lg text-base font-medium hover:bg-gray-800 transition-colors duration-300">
					Start Growing Today
				</a>
				<a href="#services" class="inline-flex items-center justify-center px-8 py-4 border border-gray-300 text-gray-900 rounded-lg text-base font-medium hover:bg-gray-50 transition-colors duration-300">
					See How We Work
				</a>
			</div>
		</div>
		
		<!-- Stats Bar -->
		<div class="mt-24 grid grid-cols-1 md:grid-cols-3 gap-8 max-w-4xl">
			<div class="text-center md:text-left">
				<div class="text-4xl md:text-5xl font-bold text-gray-900 mb-2">$6.3T</div>
				<div class="text-gray-600">E-commerce Market</div>
			</div>
			<div class="text-center md:text-left">
				<div class="text-4xl md:text-5xl font-bold text-gray-900 mb-2">20+</div>
				<div class="text-gray-600">Years Experience</div>
			</div>
			<div class="text-center md:text-left">
				<div class="text-4xl md:text-5xl font-bold text-gray-900 mb-2">50+</div>
				<div class="text-gray-600">Target Clients</div>
			</div>
		</div>
	</section>

	<!-- Platform Expertise -->
	<section class="bg-gray-50 px-6 md:px-12 lg:px-24 py-16 md:py-24">
		<p class="text-lg md:text-xl text-gray-600 mb-12 text-center">Trusted expertise across leading e-commerce platforms</p>
		
		<div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-6 gap-4 md:gap-8">
			<!-- Platform logos -->
			{#each ['Shopify', 'Shopify Plus', 'WooCommerce', 'BigCommerce', 'Magento', 'Amazon'] as platform}
				<div class="h-20 bg-white rounded-lg flex items-center justify-center grayscale opacity-70 hover:opacity-100 hover:grayscale-0 transition-all duration-300 border border-gray-200">
					<span class="font-semibold text-gray-800">{platform}</span>
				</div>
			{/each}
		</div>
	</section>

    <!-- Services Section -->
    <section class="bg-white px-6 md:px-12 lg:px-24 py-12 md:py-24" id="services">
        <div class="flex flex-col mb-16 md:mb-24">
            <h2 class="font-serif text-3xl md:text-4xl lg:text-5xl text-gray-900 mb-6">Full-stack e-commerce execution</h2>
            <p class="text-xl text-gray-600 max-w-3xl">From strategy to optimization, we manage every aspect of your platform so you can focus on what matters most—building your brand.</p>
        </div>

        <div class="space-y-24 md:space-y-32">
            <!-- Service 1: Strategy -->
            <div class="group grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
                <div class="lg:col-span-5 space-y-6">
                    <div class="inline-flex items-center justify-center w-12 h-12 bg-primary-100 text-primary-700 rounded-lg mb-4">
                        <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 19v-6a2 2 0 00-2-2H5a2 2 0 00-2 2v6a2 2 0 002 2h2a2 2 0 002-2zm0 0V9a2 2 0 012-2h2a2 2 0 012 2v10m-6 0a2 2 0 002 2h2a2 2 0 002-2m0 0V5a2 2 0 012-2h2a2 2 0 012 2v14a2 2 0 01-2 2h-2a2 2 0 01-2-2z" />
                        </svg>
                    </div>
                    <h3 class="font-serif text-3xl md:text-4xl text-gray-900">Platform Strategy</h3>
                    <p class="text-gray-600 text-lg leading-relaxed">
                        We develop comprehensive platform strategies tailored to your business goals. From selecting the right e-commerce platform to planning scalable architecture, we ensure your foundation is built for growth.
                    </p>
                    <ul class="space-y-3 text-gray-600">
                        <li class="flex items-start gap-2">
                            <svg class="w-5 h-5 text-primary-600 mt-0.5 flex-shrink-0" fill="currentColor" viewBox="0 0 20 20">
                                <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
                            </svg>
                            <span>Platform selection & migration</span>
                        </li>
                        <li class="flex items-start gap-2">
                            <svg class="w-5 h-5 text-primary-600 mt-0.5 flex-shrink-0" fill="currentColor" viewBox="0 0 20 20">
                                <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
                            </svg>
                            <span>Growth roadmap planning</span>
                        </li>
                        <li class="flex items-start gap-2">
                            <svg class="w-5 h-5 text-primary-600 mt-0.5 flex-shrink-0" fill="currentColor" viewBox="0 0 20 20">
                                <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
                            </svg>
                            <span>Technology stack optimization</span>
                        </li>
                    </ul>
                </div>
                <div class="lg:col-span-7">
                    <div class="aspect-[16/9] bg-gray-100 rounded-lg overflow-hidden relative group-hover:scale-[1.02] transition-transform duration-500 ease-out">
                        <img src="https://images.unsplash.com/photo-1460925895917-afdab827c52f?q=80&w=2000&auto=format&fit=crop" alt="Strategy planning" class="w-full h-full object-cover" />
                    </div>
                </div>
            </div>

            <!-- Service 2: Operations -->
            <div class="group grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
                <div class="lg:col-span-5 lg:order-2 space-y-6">
                    <div class="inline-flex items-center justify-center w-12 h-12 bg-primary-100 text-primary-700 rounded-lg mb-4">
                        <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10.325 4.317c.426-1.756 2.924-1.756 3.35 0a1.724 1.724 0 002.573 1.066c1.543-.94 3.31.826 2.37 2.37a1.724 1.724 0 001.065 2.572c1.756.426 1.756 2.924 0 3.35a1.724 1.724 0 00-1.066 2.573c.94 1.543-.826 3.31-2.37 2.37a1.724 1.724 0 00-2.572 1.065c-.426 1.756-2.924 1.756-3.35 0a1.724 1.724 0 00-2.573-1.066c-1.543.94-3.31-.826-2.37-2.37a1.724 1.724 0 00-1.065-2.572c-1.756-.426-1.756-2.924 0-3.35a1.724 1.724 0 001.066-2.573c-.94-1.543.826-3.31 2.37-2.37.996.608 2.296.07 2.572-1.065z" />
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 12a3 3 0 11-6 0 3 3 0 016 0z" />
                        </svg>
                    </div>
                    <h3 class="font-serif text-3xl md:text-4xl text-gray-900">Platform Operations</h3>
                    <p class="text-gray-600 text-lg leading-relaxed">
                        Hands-on execution and day-to-day platform management. We handle the technical operations so your team can focus on strategic initiatives and customer experience.
                    </p>
                    <ul class="space-y-3 text-gray-600">
                        <li class="flex items-start gap-2">
                            <svg class="w-5 h-5 text-primary-600 mt-0.5 flex-shrink-0" fill="currentColor" viewBox="0 0 20 20">
                                <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
                            </svg>
                            <span>Store setup & configuration</span>
                        </li>
                        <li class="flex items-start gap-2">
                            <svg class="w-5 h-5 text-primary-600 mt-0.5 flex-shrink-0" fill="currentColor" viewBox="0 0 20 20">
                                <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
                            </svg>
                            <span>Integration management</span>
                        </li>
                        <li class="flex items-start gap-2">
                            <svg class="w-5 h-5 text-primary-600 mt-0.5 flex-shrink-0" fill="currentColor" viewBox="0 0 20 20">
                                <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
                            </svg>
                            <span>Ongoing maintenance & support</span>
                        </li>
                    </ul>
                </div>
                <div class="lg:col-span-7 lg:order-1">
                    <div class="aspect-[16/9] bg-gray-100 rounded-lg overflow-hidden relative group-hover:scale-[1.02] transition-transform duration-500 ease-out">
                        <img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?q=80&w=2000&auto=format&fit=crop" alt="Platform operations" class="w-full h-full object-cover" />
                    </div>
                </div>
            </div>

            <!-- Service 3: Optimization -->
            <div class="group grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
                <div class="lg:col-span-5 space-y-6">
                    <div class="inline-flex items-center justify-center w-12 h-12 bg-primary-100 text-primary-700 rounded-lg mb-4">
                        <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 7h8m0 0v8m0-8l-8 8-4-4-6 6" />
                        </svg>
                    </div>
                    <h3 class="font-serif text-3xl md:text-4xl text-gray-900">Growth Optimization</h3>
                    <p class="text-gray-600 text-lg leading-relaxed">
                        Data-driven optimization to maximize revenue and profitability. We continuously analyze, test, and refine your platform to drive measurable growth.
                    </p>
                    <ul class="space-y-3 text-gray-600">
                        <li class="flex items-start gap-2">
                            <svg class="w-5 h-5 text-primary-600 mt-0.5 flex-shrink-0" fill="currentColor" viewBox="0 0 20 20">
                                <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
                            </svg>
                            <span>Conversion rate optimization</span>
                        </li>
                        <li class="flex items-start gap-2">
                            <svg class="w-5 h-5 text-primary-600 mt-0.5 flex-shrink-0" fill="currentColor" viewBox="0 0 20 20">
                                <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
                            </svg>
                            <span>Performance analytics & reporting</span>
                        </li>
                        <li class="flex items-start gap-2">
                            <svg class="w-5 h-5 text-primary-600 mt-0.5 flex-shrink-0" fill="currentColor" viewBox="0 0 20 20">
                                <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
                            </svg>
                            <span>A/B testing & experimentation</span>
                        </li>
                    </ul>
                </div>
                <div class="lg:col-span-7">
                    <div class="aspect-[16/9] bg-gray-100 rounded-lg overflow-hidden relative group-hover:scale-[1.02] transition-transform duration-500 ease-out">
                        <img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?q=80&w=2000&auto=format&fit=crop" alt="Growth optimization" class="w-full h-full object-cover" />
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Process Section -->
    <section class="bg-gray-50 px-6 md:px-12 lg:px-24 py-12 md:py-24" id="process">
        <h2 class="font-serif text-3xl md:text-4xl lg:text-5xl text-gray-900 mb-6 max-w-3xl">Our proven methodology</h2>
        <p class="text-xl text-gray-600 mb-16 max-w-3xl">Built on 20+ years of experience with multi-million dollar e-commerce brands</p>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
            <!-- Discover -->
            <div class="bg-white p-8 rounded-xl border border-gray-200 hover:border-primary-300 transition-all duration-300 flex flex-col h-full">
                <div class="w-12 h-12 bg-primary-100 text-primary-700 rounded-lg flex items-center justify-center mb-6">
                    <span class="text-2xl font-bold">1</span>
                </div>
                <h3 class="text-2xl font-semibold mb-4">Discover</h3>
                <p class="text-gray-600 leading-relaxed mb-6">
                    We analyze your current platform, business goals, and market position to identify opportunities for growth and optimization.
                </p>
                <ul class="space-y-2 text-sm text-gray-600">
                    <li class="flex items-start gap-2">
                        <span class="text-primary-600 mt-1">•</span>
                        <span>Platform audit</span>
                    </li>
                    <li class="flex items-start gap-2">
                        <span class="text-primary-600 mt-1">•</span>
                        <span>Competitive analysis</span>
                    </li>
                    <li class="flex items-start gap-2">
                        <span class="text-primary-600 mt-1">•</span>
                        <span>Growth opportunity mapping</span>
                    </li>
                </ul>
            </div>

            <!-- Execute -->
            <div class="bg-white p-8 rounded-xl border border-gray-200 hover:border-primary-300 transition-all duration-300 flex flex-col h-full">
                <div class="w-12 h-12 bg-primary-100 text-primary-700 rounded-lg flex items-center justify-center mb-6">
                    <span class="text-2xl font-bold">2</span>
                </div>
                <h3 class="text-2xl font-semibold mb-4">Execute</h3>
                <p class="text-gray-600 leading-relaxed mb-6">
                    We implement strategic initiatives with hands-on execution, managing every detail of your platform operations and optimization.
                </p>
                <ul class="space-y-2 text-sm text-gray-600">
                    <li class="flex items-start gap-2">
                        <span class="text-primary-600 mt-1">•</span>
                        <span>Platform configuration</span>
                    </li>
                    <li class="flex items-start gap-2">
                        <span class="text-primary-600 mt-1">•</span>
                        <span>Integration setup</span>
                    </li>
                    <li class="flex items-start gap-2">
                        <span class="text-primary-600 mt-1">•</span>
                        <span>Process implementation</span>
                    </li>
                </ul>
            </div>

            <!-- Scale -->
            <div class="bg-white p-8 rounded-xl border border-gray-200 hover:border-primary-300 transition-all duration-300 flex flex-col h-full">
                <div class="w-12 h-12 bg-primary-100 text-primary-700 rounded-lg flex items-center justify-center mb-6">
                    <span class="text-2xl font-bold">3</span>
                </div>
                <h3 class="text-2xl font-semibold mb-4">Scale</h3>
                <p class="text-gray-600 leading-relaxed mb-6">
                    We continuously optimize and scale your operations, using data-driven insights to drive profitable growth month over month.
                </p>
                <ul class="space-y-2 text-sm text-gray-600">
                    <li class="flex items-start gap-2">
                        <span class="text-primary-600 mt-1">•</span>
                        <span>Performance monitoring</span>
                    </li>
                    <li class="flex items-start gap-2">
                        <span class="text-primary-600 mt-1">•</span>
                        <span>Continuous optimization</span>
                    </li>
                    <li class="flex items-start gap-2">
                        <span class="text-primary-600 mt-1">•</span>
                        <span>Revenue growth tracking</span>
                    </li>
                </ul>
            </div>
        </div>
    </section>

    <!-- Results Section -->
    <section class="bg-white px-6 md:px-12 lg:px-24 py-12 md:py-24" id="results">
        <div class="flex flex-col mb-12">
            <h2 class="font-serif text-3xl md:text-4xl text-gray-900 mb-4">Proven results that drive growth</h2>
            <p class="text-xl text-gray-600 max-w-3xl">Real revenue growth from our portfolio of e-commerce case studies</p>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-8 mb-16">
            <!-- Result 1 -->
            <div class="bg-gray-50 p-8 rounded-xl border border-gray-200">
                <div class="text-5xl font-bold text-primary-600 mb-4">+247%</div>
                <h3 class="text-lg font-semibold text-gray-900 mb-2">Revenue Growth</h3>
                <p class="text-gray-600 text-sm">Fashion brand scaled from $2M to $7M ARR through platform optimization and strategic execution</p>
            </div>

            <!-- Result 2 -->
            <div class="bg-gray-50 p-8 rounded-xl border border-gray-200">
                <div class="text-5xl font-bold text-primary-600 mb-4">+185%</div>
                <h3 class="text-lg font-semibold text-gray-900 mb-2">Conversion Rate</h3>
                <p class="text-gray-600 text-sm">Home goods retailer improved checkout conversion from 1.2% to 3.4% through UX optimization</p>
            </div>

            <!-- Result 3 -->
            <div class="bg-gray-50 p-8 rounded-xl border border-gray-200">
                <div class="text-5xl font-bold text-primary-600 mb-4">-42%</div>
                <h3 class="text-lg font-semibold text-gray-900 mb-2">Operational Costs</h3>
                <p class="text-gray-600 text-sm">B2B distributor reduced platform costs while scaling operations through strategic integrations</p>
            </div>
        </div>

        <!-- Testimonials -->
        <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
            <!-- Testimonial 1 -->
            <div class="bg-gray-900 p-8 md:p-12 rounded-xl text-white">
                <div class="flex items-start gap-1 mb-6">
                    {#each [1, 2, 3, 4, 5] as star}
                        <svg class="w-5 h-5 text-primary-400" fill="currentColor" viewBox="0 0 20 20">
                            <path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z" />
                        </svg>
                    {/each}
                </div>
                <p class="text-lg mb-6 leading-relaxed">
                    "Working with Eightyfour Commerce transformed our e-commerce operations. Their expertise in Shopify Plus helped us scale from $3M to $10M in just 18 months. They handle everything so we can focus on our brand."
                </p>
                <div class="flex items-center gap-4">
                    <div class="w-12 h-12 bg-primary-600 rounded-full flex items-center justify-center text-white font-bold">
                        SM
                    </div>
                    <div>
                        <div class="font-semibold">Sarah Mitchell</div>
                        <div class="text-sm text-gray-400">CEO, Fashion Brand</div>
                    </div>
                </div>
            </div>

            <!-- Testimonial 2 -->
            <div class="bg-primary-50 p-8 md:p-12 rounded-xl">
                <div class="flex items-start gap-1 mb-6">
                    {#each [1, 2, 3, 4, 5] as star}
                        <svg class="w-5 h-5 text-primary-600" fill="currentColor" viewBox="0 0 20 20">
                            <path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z" />
                        </svg>
                    {/each}
                </div>
                <p class="text-lg mb-6 leading-relaxed text-gray-900">
                    "The level of expertise and hands-on support is unmatched. They don't just consult—they execute. Our conversion rates doubled and our platform runs smoother than ever. Best investment we've made."
                </p>
                <div class="flex items-center gap-4">
                    <div class="w-12 h-12 bg-primary-600 rounded-full flex items-center justify-center text-white font-bold">
                        JC
                    </div>
                    <div>
                        <div class="font-semibold text-gray-900">James Chen</div>
                        <div class="text-sm text-gray-600">Founder, Home Goods Co.</div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Newsletter Section -->
    <section class="px-6 md:px-12 lg:px-24 py-12 bg-gray-50">
        <div class="bg-white border border-gray-200 rounded-2xl p-8 md:p-16 lg:p-20">
            <h3 class="font-serif text-2xl md:text-3xl text-gray-900 mb-4">Get e-commerce insights delivered monthly</h3>
            <p class="text-gray-600 mb-8 max-w-md">Platform strategies, optimization tips, and growth tactics from 20+ years of e-commerce experience.</p>
            
            <form class="flex flex-col sm:flex-row gap-4 max-w-lg">
                <input type="email" placeholder="your@email.com" class="flex-1 bg-gray-50 border border-gray-300 rounded-lg px-4 py-3 text-sm placeholder:text-gray-400 focus:ring-2 focus:ring-primary-500 focus:border-transparent outline-none" />
                <button type="submit" class="bg-gray-900 hover:bg-gray-800 transition-colors text-white px-8 py-3 rounded-lg text-sm font-medium">
                    Subscribe
                </button>
            </form>
            <p class="text-xs text-gray-500 mt-4">We respect your privacy. Unsubscribe anytime.</p>
        </div>
    </section>

    <!-- CTA Section -->
    <section class="relative bg-gray-900 pt-24 pb-32 px-6 md:px-12 lg:px-24 overflow-hidden" id="contact">
        <div class="max-w-4xl relative z-10">
            <h2 class="font-serif text-4xl md:text-5xl lg:text-6xl text-white leading-tight mb-6">
                Ready to drive profitable growth?
            </h2>
            <p class="text-xl text-gray-300 mb-12 max-w-2xl">
                Let's discuss how our platform management expertise can help scale your e-commerce brand. With 20+ years of experience, we know what works.
            </p>
            
            <div class="flex flex-col sm:flex-row gap-4">
                <a href="mailto:hello@eightyfourcommerce.com" class="inline-flex items-center justify-center px-8 py-4 bg-primary-600 text-white rounded-lg text-base font-medium hover:bg-primary-700 transition-colors duration-300">
                    Get in Touch
                </a>
                <a href="#services" class="inline-flex items-center justify-center px-8 py-4 border border-white/30 text-white rounded-lg text-base font-medium hover:bg-white/10 transition-colors duration-300">
                    Learn More
                </a>
            </div>
        </div>
        
        <!-- Background Pattern -->
        <div class="absolute inset-0 opacity-5">
            <div class="absolute inset-0" style="background-image: url('data:image/svg+xml,%3Csvg width=&quot;60&quot; height=&quot;60&quot; viewBox=&quot;0 0 60 60&quot; xmlns=&quot;http://www.w3.org/2000/svg&quot;%3E%3Cg fill=&quot;none&quot; fill-rule=&quot;evenodd&quot;%3E%3Cg fill=&quot;%23ffffff&quot; fill-opacity=&quot;1&quot;%3E%3Cpath d=&quot;M36 34v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zm0-30V0h-2v4h-4v2h4v4h2V6h4V4h-4zM6 34v-4H4v4H0v2h4v4h2v-4h4v-2H6zM6 4V0H4v4H0v2h4v4h2V6h4V4H6z&quot;/%3E%3C/g%3E%3C/g%3E%3C/svg%3E');"></div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-950 text-gray-400 px-6 md:px-12 lg:px-24 pt-16 pb-8 relative overflow-hidden">
        <div class="relative z-10">
            <div class="grid grid-cols-1 md:grid-cols-3 gap-12 mb-16">
                <div class="col-span-1 md:col-span-1">
                    <div class="flex items-center gap-2 mb-6">
                        <svg class="w-8 h-8 text-white" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path
                                fill-rule="evenodd"
                                clip-rule="evenodd"
                                d="M5.0473 17.8386L5.69453 18.9586V18.9601H18.3003L18.9314 17.84H6.34063L6.82626 16.9993H19.4308L20.078 15.8807H7.47237L7.95715 15.0414H16.0358L16.0366 15.0429L16.0375 15.0414H20.5603L20.5612 15.0429L21.2084 13.9228L21.208 13.922L21.2084 13.9213H21.2075L14.9084 3.00677L14.9106 3.00296L14.9062 3.00296L13.6177 3.00296L5.0473 17.8386ZM14.261 4.12767L13.7751 4.96887L18.9438 13.9213H19.9139L14.261 4.12767ZM13.1286 6.08808L12.6467 6.9225L16.6749 13.9006L16.6634 13.9213H17.6511L13.1286 6.08808ZM11.9999 8.04225L8.60411 13.9213H15.3899L11.9999 8.04225ZM6.99833 3.30006C7.33866 3.10343 7.7248 2.99993 8.11786 3L2.30033 13.0776C2.10357 12.7371 2 12.3508 2 11.9575C2 11.5643 2.10357 11.178 2.30033 10.8375L6.17916 4.12006C6.37543 3.77951 6.65798 3.49669 6.99833 3.30006ZM9.08869 3H10.3816L3.43223 15.0384L2.785 13.9184L9.08869 3ZM11.3509 3H12.6424L4.56262 16.9963L3.91691 15.8777L11.3509 3ZM21.7064 13.0598C21.8988 12.7254 22 12.3463 22 11.9605C22 11.5746 21.8988 11.1956 21.7064 10.8611L17.8039 4.10233C17.6108 3.7681 17.3331 3.49057 16.9987 3.2976C16.6644 3.10463 16.2852 3.00302 15.8992 3.00296H15.8741L21.6931 13.082L21.7064 13.0598ZM17.7995 19.7994H6.17916C6.37472 20.1412 6.65692 20.4253 6.99728 20.6232C7.33763 20.8212 7.72414 20.9258 8.11786 20.9269H15.8829C16.2737 20.9261 16.6572 20.8212 16.994 20.6231C17.3309 20.4249 17.6089 20.1406 17.7995 19.7994Z"
                                fill="currentColor"
                            />
                        </svg>
                        <span class="font-semibold text-lg text-white">Eightyfour Commerce</span>
                    </div>
                    <p class="text-sm mb-6">
                        Expert e-commerce platform management for brands that want to scale profitably.
                    </p>
                </div>
                
                <div class="space-y-4">
                    <h4 class="font-medium text-white mb-4">Services</h4>
                    <div class="space-y-2 text-sm">
                        <a href="#services" class="block hover:text-white transition-colors">Platform Strategy</a>
                        <a href="#services" class="block hover:text-white transition-colors">Platform Operations</a>
                        <a href="#services" class="block hover:text-white transition-colors">Growth Optimization</a>
                        <a href="#process" class="block hover:text-white transition-colors">Our Process</a>
                    </div>
                </div>

                <div class="space-y-4">
                    <h4 class="font-medium text-white mb-4">Contact</h4>
                    <div class="text-sm space-y-2">
                        <p>
                            <a href="mailto:hello@eightyfourcommerce.com" class="hover:text-white transition-colors">
                                hello@eightyfourcommerce.com
                            </a>
                        </p>
                        <p class="pt-4">
                            Shopify Partner Directory<br>
                            Trusted by e-commerce brands worldwide
                        </p>
                    </div>
                </div>
            </div>

            <div class="flex flex-col md:flex-row justify-between items-center border-t border-gray-800 pt-8 gap-4">
                <div class="text-xs">
                    © 2025 Eightyfour Commerce. All rights reserved.
                </div>
                
                <div class="flex gap-6 text-xs">
                    <a href="#" class="hover:text-white transition-colors">LinkedIn</a>
                    <a href="#" class="hover:text-white transition-colors">Privacy Policy</a>
                    <a href="#" class="hover:text-white transition-colors">Terms of Service</a>
                </div>
            </div>
        </div>
    </footer>
</div>

<style>
    /* Custom utility for vertical writing mode */
    .writing-vertical-rl {
        writing-mode: vertical-rl;
    }
</style>

