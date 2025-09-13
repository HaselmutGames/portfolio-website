<script lang="ts">
	import '../app.css';
</script>

<header class="w-full bg-gray-900 shadow">
	<nav class="mx-auto flex max-w-6xl items-center justify-between p-6">
		<!-- Logo / Name -->
		<a href="/" class="text-xl font-bold tracking-tight text-gray-400 hover:text-gray-200">
			HaselmutGames
		</a>

		<!-- Nav Links -->
		<ul
			class="flex gap-8 text-lg max-md:absolute max-md:top-full max-md:right-0 max-md:hidden
               max-md:flex-col max-md:bg-gray-900 max-md:p-4 max-md:shadow-md"
		>
			<li><a href="/projects" class="text-gray-400 hover:text-gray-200">Projects</a></li>
			<li><a href="/experience" class="text-gray-400 hover:text-gray-200">Experience</a></li>
			<li><a href="/stream" class="text-gray-400 hover:text-gray-200">Stream</a></li>
			<li><a href="/contact" class="text-gray-400 hover:text-gray-200">Contact</a></li>
		</ul>
	</nav>
</header>

<main id="main" class="mx-auto max-w-6xl p-6">
	<slot />
	<!-- Each page renders here -->
</main>

<footer class="mt-16 w-full bg-gray-900">
	<div class="mx-auto max-w-6xl p-6 text-center text-sm text-gray-400">
		© {new Date().getFullYear()} HaselmutGames — All Rights Reserved
	</div>
</footer>
