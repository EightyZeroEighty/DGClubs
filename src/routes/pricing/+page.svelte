<script>
	/** @type {{ data: import('./$types').PageData }} */
	let { data } = $props();
</script>

<!-- Header Section -->
<div class="bg-gradient-to-r from-blue-600 to-blue-800 text-white">
	<div class="mx-auto max-w-7xl px-4 py-24 sm:px-6 lg:px-8">
		<div class="text-center">
			<h1 class="mb-6 text-4xl font-bold md:text-5xl">Simple, Transparent Pricing</h1>
			<p class="mx-auto mb-8 max-w-2xl text-xl text-blue-100">
				Choose the plan that fits your club's needs. All plans include our core features with no
				hidden fees.
			</p>
			<div class="inline-flex items-center rounded-lg bg-blue-700 p-1">
				<button class="rounded-md bg-white px-4 py-2 text-sm font-medium text-blue-600"
					>Monthly</button
				>
				<button class="rounded-md px-4 py-2 text-sm font-medium text-blue-100"
					>Annual (Save 20%)</button
				>
			</div>
		</div>
	</div>
</div>

<!-- Pricing Cards -->
<div class="mx-auto mt-8 max-w-7xl px-4 sm:px-6 lg:px-8">
	<div class="grid gap-8 lg:grid-cols-3">
		<!-- Basic Plan -->
		<div class="overflow-hidden rounded-lg bg-white shadow-lg">
			<div class="p-6">
				<h2 class="text-2xl font-bold text-gray-800">Basic</h2>
				<p class="mt-2 text-gray-600">Perfect for small clubs getting started</p>
				<div class="mt-4">
					<span class="text-4xl font-bold">$29</span>
					<span class="text-gray-600">/month</span>
				</div>
				<a
					href="#signup"
					class="mt-6 block w-full rounded-lg bg-blue-600 py-3 text-center text-white hover:bg-blue-700"
				>
					Start Free Trial
				</a>
			</div>
			<div class="border-t border-gray-100 p-6">
				<ul class="space-y-4">
					<li class="flex items-start">
						<svg
							class="mt-1 h-5 w-5 flex-shrink-0 text-green-500"
							fill="none"
							stroke="currentColor"
							viewBox="0 0 24 24"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M5 13l4 4L19 7"
							></path>
						</svg>
						<span class="ml-3 text-gray-600">Single course management</span>
					</li>
					<li class="flex items-start">
						<svg
							class="mt-1 h-5 w-5 flex-shrink-0 text-green-500"
							fill="none"
							stroke="currentColor"
							viewBox="0 0 24 24"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M5 13l4 4L19 7"
							></path>
						</svg>
						<span class="ml-3 text-gray-600">Up to 50 active members</span>
					</li>
					<li class="flex items-start">
						<svg
							class="mt-1 h-5 w-5 flex-shrink-0 text-green-500"
							fill="none"
							stroke="currentColor"
							viewBox="0 0 24 24"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M5 13l4 4L19 7"
							></path>
						</svg>
						<span class="ml-3 text-gray-600">Basic event management</span>
					</li>
					<li class="flex items-start">
						<svg
							class="mt-1 h-5 w-5 flex-shrink-0 text-green-500"
							fill="none"
							stroke="currentColor"
							viewBox="0 0 24 24"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M5 13l4 4L19 7"
							></path>
						</svg>
						<span class="ml-3 text-gray-600">Email notifications</span>
					</li>
					<li class="flex items-start">
						<svg
							class="mt-1 h-5 w-5 flex-shrink-0 text-green-500"
							fill="none"
							stroke="currentColor"
							viewBox="0 0 24 24"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M5 13l4 4L19 7"
							></path>
						</svg>
						<span class="ml-3 text-gray-600">Basic reporting</span>
					</li>
				</ul>
			</div>
		</div>

		<!-- Pro Plan -->
		<div class="relative overflow-hidden rounded-lg bg-white shadow-lg lg:scale-105">
			<div
				class="absolute right-0 top-0 rounded-bl-lg bg-blue-600 px-3 py-1 text-sm font-medium text-white"
			>
				Most Popular
			</div>
			<div class="p-6">
				<h2 class="text-2xl font-bold text-gray-800">Pro</h2>
				<p class="mt-2 text-gray-600">For growing clubs with multiple courses</p>
				<div class="mt-4">
					<span class="text-4xl font-bold">$79</span>
					<span class="text-gray-600">/month</span>
				</div>
				<a
					href="#signup"
					class="mt-6 block w-full rounded-lg bg-blue-600 py-3 text-center text-white hover:bg-blue-700"
				>
					Start Free Trial
				</a>
			</div>
			<div class="border-t border-gray-100 p-6">
				<ul class="space-y-4">
					<li class="flex items-start">
						<svg
							class="mt-1 h-5 w-5 flex-shrink-0 text-green-500"
							fill="none"
							stroke="currentColor"
							viewBox="0 0 24 24"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M5 13l4 4L19 7"
							></path>
						</svg>
						<span class="ml-3 text-gray-600">Everything in Basic, plus:</span>
					</li>
					<li class="flex items-start">
						<svg
							class="mt-1 h-5 w-5 flex-shrink-0 text-green-500"
							fill="none"
							stroke="currentColor"
							viewBox="0 0 24 24"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M5 13l4 4L19 7"
							></path>
						</svg>
						<span class="ml-3 text-gray-600">Up to 3 courses</span>
					</li>
					<li class="flex items-start">
						<svg
							class="mt-1 h-5 w-5 flex-shrink-0 text-green-500"
							fill="none"
							stroke="currentColor"
							viewBox="0 0 24 24"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M5 13l4 4L19 7"
							></path>
						</svg>
						<span class="ml-3 text-gray-600">Up to 200 active members</span>
					</li>
					<li class="flex items-start">
						<svg
							class="mt-1 h-5 w-5 flex-shrink-0 text-green-500"
							fill="none"
							stroke="currentColor"
							viewBox="0 0 24 24"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M5 13l4 4L19 7"
							></path>
						</svg>
						<span class="ml-3 text-gray-600">Advanced event management</span>
					</li>
					<li class="flex items-start">
						<svg
							class="mt-1 h-5 w-5 flex-shrink-0 text-green-500"
							fill="none"
							stroke="currentColor"
							viewBox="0 0 24 24"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M5 13l4 4L19 7"
							></path>
						</svg>
						<span class="ml-3 text-gray-600">Financial tools & payments</span>
					</li>
					<li class="flex items-start">
						<svg
							class="mt-1 h-5 w-5 flex-shrink-0 text-green-500"
							fill="none"
							stroke="currentColor"
							viewBox="0 0 24 24"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M5 13l4 4L19 7"
							></path>
						</svg>
						<span class="ml-3 text-gray-600">SMS notifications</span>
					</li>
					<li class="flex items-start">
						<svg
							class="mt-1 h-5 w-5 flex-shrink-0 text-green-500"
							fill="none"
							stroke="currentColor"
							viewBox="0 0 24 24"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M5 13l4 4L19 7"
							></path>
						</svg>
						<span class="ml-3 text-gray-600">Advanced analytics</span>
					</li>
				</ul>
			</div>
		</div>

		<!-- Enterprise Plan -->
		<div class="overflow-hidden rounded-lg bg-white shadow-lg">
			<div class="p-6">
				<h2 class="text-2xl font-bold text-gray-800">Enterprise</h2>
				<p class="mt-2 text-gray-600">For large clubs and organizations</p>
				<div class="mt-4">
					<span class="text-4xl font-bold">Custom</span>
				</div>
				<a
					href="#contact"
					class="mt-6 block w-full rounded-lg bg-blue-600 py-3 text-center text-white hover:bg-blue-700"
				>
					Contact Sales
				</a>
			</div>
			<div class="border-t border-gray-100 p-6">
				<ul class="space-y-4">
					<li class="flex items-start">
						<svg
							class="mt-1 h-5 w-5 flex-shrink-0 text-green-500"
							fill="none"
							stroke="currentColor"
							viewBox="0 0 24 24"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M5 13l4 4L19 7"
							></path>
						</svg>
						<span class="ml-3 text-gray-600">Everything in Pro, plus:</span>
					</li>
					<li class="flex items-start">
						<svg
							class="mt-1 h-5 w-5 flex-shrink-0 text-green-500"
							fill="none"
							stroke="currentColor"
							viewBox="0 0 24 24"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M5 13l4 4L19 7"
							></path>
						</svg>
						<span class="ml-3 text-gray-600">Unlimited courses</span>
					</li>
					<li class="flex items-start">
						<svg
							class="mt-1 h-5 w-5 flex-shrink-0 text-green-500"
							fill="none"
							stroke="currentColor"
							viewBox="0 0 24 24"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M5 13l4 4L19 7"
							></path>
						</svg>
						<span class="ml-3 text-gray-600">Unlimited members</span>
					</li>
					<li class="flex items-start">
						<svg
							class="mt-1 h-5 w-5 flex-shrink-0 text-green-500"
							fill="none"
							stroke="currentColor"
							viewBox="0 0 24 24"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M5 13l4 4L19 7"
							></path>
						</svg>
						<span class="ml-3 text-gray-600">Custom branding</span>
					</li>
					<li class="flex items-start">
						<svg
							class="mt-1 h-5 w-5 flex-shrink-0 text-green-500"
							fill="none"
							stroke="currentColor"
							viewBox="0 0 24 24"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M5 13l4 4L19 7"
							></path>
						</svg>
						<span class="ml-3 text-gray-600">API access</span>
					</li>
					<li class="flex items-start">
						<svg
							class="mt-1 h-5 w-5 flex-shrink-0 text-green-500"
							fill="none"
							stroke="currentColor"
							viewBox="0 0 24 24"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M5 13l4 4L19 7"
							></path>
						</svg>
						<span class="ml-3 text-gray-600">Priority support</span>
					</li>
					<li class="flex items-start">
						<svg
							class="mt-1 h-5 w-5 flex-shrink-0 text-green-500"
							fill="none"
							stroke="currentColor"
							viewBox="0 0 24 24"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M5 13l4 4L19 7"
							></path>
						</svg>
						<span class="ml-3 text-gray-600">Dedicated account manager</span>
					</li>
				</ul>
			</div>
		</div>
	</div>
	<!-- FAQ Section -->
	<div class="mt-8">
		<h2 class="mb-12 text-center text-3xl font-bold">Frequently Asked Questions</h2>
		<div class="mx-auto max-w-3xl space-y-8">
			<!-- Question 1 -->
			<div class="rounded-lg bg-white p-6 shadow-sm">
				<h3 class="mb-2 text-lg font-semibold text-gray-800">Can I switch plans at any time?</h3>
				<p class="text-gray-600">
					Yes, you can upgrade or downgrade your plan at any time. When upgrading, the new features
					will be immediately available. When downgrading, the changes will take effect at the start
					of your next billing cycle.
				</p>
			</div>

			<!-- Question 2 -->
			<div class="rounded-lg bg-white p-6 shadow-sm">
				<h3 class="mb-2 text-lg font-semibold text-gray-800">Is there a free trial available?</h3>
				<p class="text-gray-600">
					Yes, we offer a 14-day free trial for both our Basic and Pro plans. No credit card is
					required to start your trial, and you can explore all features risk-free.
				</p>
			</div>

			<!-- Question 3 -->
			<div class="rounded-lg bg-white p-6 shadow-sm">
				<h3 class="mb-2 text-lg font-semibold text-gray-800">
					What payment methods do you accept?
				</h3>
				<p class="text-gray-600">
					We accept all major credit cards (Visa, MasterCard, American Express) and can also
					accommodate ACH payments for Enterprise customers. All payments are processed securely
					through Stripe.
				</p>
			</div>

			<!-- Question 4 -->
			<div class="rounded-lg bg-white p-6 shadow-sm">
				<h3 class="mb-2 text-lg font-semibold text-gray-800">How does the annual discount work?</h3>
				<p class="text-gray-600">
					When you choose annual billing, you'll receive a 20% discount compared to monthly billing.
					The annual amount is billed once upfront for the entire year.
				</p>
			</div>

			<!-- Question 5 -->
			<div class="rounded-lg bg-white p-6 shadow-sm">
				<h3 class="mb-2 text-lg font-semibold text-gray-800">What kind of support is included?</h3>
				<p class="text-gray-600">
					All plans include email support with 24-hour response time. Pro plans include priority
					email support with 4-hour response time. Enterprise plans include dedicated support with
					phone access and a dedicated account manager.
				</p>
			</div>
		</div>
	</div>

	<!-- Bottom CTA -->
	<div class="bg-gray-50 py-16 text-center">
		<h2 class="mb-4 text-2xl font-bold text-gray-800">Ready to get started?</h2>
		<p class="mb-8 text-gray-600">Start your 14-day free trial today. No credit card required.</p>
		<div class="space-x-4">
			<a
				href="#signup"
				class="inline-block rounded-lg bg-blue-600 px-8 py-3 text-white hover:bg-blue-700"
			>
				Start Free Trial
			</a>
			<a
				href="#demo"
				class="inline-block rounded-lg border border-blue-600 bg-white px-8 py-3 text-blue-600 hover:bg-gray-50"
			>
				Request Demo
			</a>
		</div>
		<p class="mt-6 text-sm text-gray-500">
			Need help choosing the right plan?
			<a href="#contact" class="text-blue-600 hover:text-blue-700">Contact our sales team</a>
		</p>
	</div>

	<!-- Feature Comparison Table (Mobile Hidden) -->
	<div class="mt-24 hidden lg:block">
		<h2 class="mb-12 text-center text-3xl font-bold">Full Feature Comparison</h2>
		<div class="mx-auto max-w-6xl">
			<table class="w-full border-collapse">
				<thead>
					<tr class="bg-gray-50">
						<th class="border-b p-4 text-left">Feature</th>
						<th class="border-b p-4 text-center">Basic</th>
						<th class="border-b p-4 text-center">Pro</th>
						<th class="border-b p-4 text-center">Enterprise</th>
					</tr>
				</thead>
				<tbody class="bg-white">
					<tr>
						<td class="border-b p-4 font-medium">Courses</td>
						<td class="border-b p-4 text-center">1</td>
						<td class="border-b p-4 text-center">Up to 3</td>
						<td class="border-b p-4 text-center">Unlimited</td>
					</tr>
					<tr>
						<td class="border-b p-4 font-medium">Active Members</td>
						<td class="border-b p-4 text-center">50</td>
						<td class="border-b p-4 text-center">200</td>
						<td class="border-b p-4 text-center">Unlimited</td>
					</tr>
					<tr>
						<td class="border-b p-4 font-medium">Support Response Time</td>
						<td class="border-b p-4 text-center">24 hours</td>
						<td class="border-b p-4 text-center">4 hours</td>
						<td class="border-b p-4 text-center">1 hour</td>
					</tr>
					<tr>
						<td class="border-b p-4 font-medium">Custom Branding</td>
						<td class="border-b p-4 text-center">❌</td>
						<td class="border-b p-4 text-center">❌</td>
						<td class="border-b p-4 text-center">✅</td>
					</tr>
					<tr>
						<td class="border-b p-4 font-medium">API Access</td>
						<td class="border-b p-4 text-center">❌</td>
						<td class="border-b p-4 text-center">❌</td>
						<td class="border-b p-4 text-center">✅</td>
					</tr>
				</tbody>
			</table>
		</div>
	</div>
</div>
