<script>
	import '../app.css';
	let { children } = $props();
	let currentYear = new Date().getFullYear();
</script>

<nav
	class="sticky top-0 z-50 flex justify-between bg-white px-4 py-4 shadow-md lg:border-b lg:px-6 lg:shadow-none"
>
	<a href="/"><img src="/logo.svg" alt="TS" /></a>
	<ul class="flex justify-end space-x-4 lg:space-x-6">
		<li><a href="/projects">Projects</a></li>
		<li><a href="/courses">Courses</a></li>
		<li><a href="/about">About</a></li>
	</ul>
</nav>

{@render children()}

<footer class="my-4 py-3">
	<p class="text-muted text-center text-gray-500">
		<small>
			&copy; {currentYear} Tarun Samant
		</small>
	</p>
</footer>
