<script lang="ts">
	import ProfileImage0 from '$lib/assets/images/profile_0.jpg?enhanced';
	import ProfileImage1 from '$lib/assets/images/profile_1.png?enhanced';

	function handleImageError(event: Event) {
		const target = event.target as HTMLImageElement;
		target.onerror = null;
		target.src = 'https://placehold.co/160x160/27272a/d4d4d8?text=Coming Soon';
	}
</script>

<svelte:head>
	<title>Tegar Aditya - Portfolio</title>
	<meta name="description" content="Portfolio of Tegar Aditya, a passionate Fullstack Web Developer specializing in PHP, JavaScript, TypeScript, Golang, and Rust. Building scalable APIs and web applications." />
	<meta name="keywords" content="Tegar Aditya, portfolio, web developer, fullstack, PHP, JavaScript, TypeScript, Golang, Rust, API development, web applications, backend, frontend" />
	<meta property="og:title" content="Tegar Aditya | Fullstack Web Developer Portfolio" />
	<meta property="og:description" content="Discover the work of Tegar Aditya, a skilled Fullstack Web Developer creating scalable and efficient web solutions."/>
	<meta property="og:image" content={ProfileImage1.img.src} />
	<meta property="og:url" content="https://tegar.dev/" />
	<meta property="og:type" content="website" />
	<meta name="twitter:card" content="summary_large_image" />
	<meta name="twitter:title" content="Tegar Aditya | Fullstack Web Developer Portfolio" />
	<meta name="twitter:description" content="Discover the work of Tegar Aditya, a skilled Fullstack Web Developer creating scalable and efficient web solutions." />
	<meta name="twitter:image" content={ProfileImage1.img.src} />
	<meta name="author" content="Tegar Aditya" />
	<link rel="canonical" href="https://tegar.dev/" />
</svelte:head>

<div class="flex-grow">
	<header class="mb-12 flex flex-col items-center md:flex-row">
		<div class="flip-container mb-6 h-32 w-32 flex-shrink-0 md:mr-8 md:mb-0 md:h-40 md:w-40">
			<div class="flipper">
				<div class="front">
					<enhanced:img
						class="h-full w-full rounded-full border-4 border-zinc-700 object-cover shadow-lg"
						sizes="(min-width: 768px) 320px, (min-width: 640px) 240px, 160px"
						src={ProfileImage1}
						alt="Tegar Aditya."
						on:error={handleImageError}
					/>
				</div>
				<div class="back">
					<enhanced:img
						class="h-full w-full rounded-full border-4 border-zinc-700 object-cover shadow-lg"
						sizes="(min-width: 768px) 320px, (min-width: 640px) 240px, 160px"
						src={ProfileImage0}
						alt="Alternative view of Tegar Aditya."
						on:error={handleImageError}
					/>
				</div>
			</div>
		</div>
		<div>
			<h1
				class="mb-2 text-center font-display text-3xl font-bold text-white md:text-left md:text-4xl"
			>
				Hi there, I'm Tegar Aditya! 👋
			</h1>
			<p class="text-md text-center text-zinc-400 italic md:text-left md:text-lg">
				"Building Scalable APIs & Fullstack Web Application | Deployment & Automation Enthusiast"
			</p>
		</div>
	</header>
	<main class="space-y-6 text-sm leading-relaxed md:text-base">
		<p>
			Hello! My name is Tegar Aditya, a dedicated and passionate web developer. I thrive on
			transforming complex ideas into functional and user-friendly web applications. My journey in
			programming has led me to specialize primarily in the robust world of
			<span class="font-medium text-white">PHP</span>
			and the dynamic <span class="font-medium text-white">JavaScript</span> ecosystem, which
			includes extensive experience with <span class="font-medium text-white">TypeScript</span> for building
			scalable and maintainable front-end and back-end solutions.
		</p>
		<p>
			Beyond my core expertise, I am constantly exploring and integrating new technologies to
			enhance performance and solve challenging problems. This includes leveraging the power of
			<span class="font-medium text-white">Golang</span>
			for high-performance microservices and server-side operations, and utilizing
			<span class="font-medium text-white">Rust</span> when efficiency, safety, and concurrency are paramount,
			particularly in performance-critical web components or system-level tools that support web applications.
		</p>
		<p>
			I'm always eager to learn, contribute, and collaborate on exciting projects that push the
			boundaries of web development. Feel free to explore my repositories and reach out if you have
			an interesting idea or just want to connect!
		</p>
	</main>

	<footer class="mt-12 text-center text-zinc-400">
		<div class="mb-4 flex flex-wrap justify-center gap-x-6 gap-y-4 text-sm">
			<a
				href="https://github.com/TegarAditya"
				target="_blank"
				class="flex items-center space-x-2 text-zinc-400 transition-colors hover:text-white"
			>
				<svg class="h-5 w-5" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true">
					<path
						fill-rule="evenodd"
						d="M12 2C6.477 2 2 6.477 2 12c0 4.418 2.865 8.168 6.839 9.492.5.092.682-.217.682-.482 0-.237-.009-.868-.014-1.703-2.782.605-3.369-1.343-3.369-1.343-.454-1.158-1.11-1.466-1.11-1.466-.908-.62.069-.608.069-.608 1.003.07 1.531 1.032 1.531 1.032.892 1.53 2.341 1.088 2.91.832.092-.647.35-1.088.636-1.338-2.22-.253-4.555-1.113-4.555-4.951 0-1.093.39-1.988 1.031-2.688-.103-.253-.446-1.272.098-2.65 0 0 .84-.27 2.75 1.026A9.564 9.564 0 0112 6.844c.85.004 1.705.115 2.504.337 1.909-1.296 2.747-1.027 2.747-1.027.546 1.378.203 2.398.1 2.65.64.7 1.028 1.595 1.028 2.688 0 3.848-2.338 4.695-4.566 4.943.359.309.678.92.678 1.855 0 1.338-.012 2.419-.012 2.747 0 .268.18.58.688.482A10.001 10.001 0 0022 12c0-5.523-4.477-10-10-10z"
						clip-rule="evenodd"
					/>
				</svg>
				<span>GitHub</span>
			</a>
			<a
				href="https://linkedin.com/in/tegar-aditya/"
				target="_blank"
				class="flex items-center space-x-2 text-zinc-400 transition-colors hover:text-white"
			>
				<svg class="h-5 w-5" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true">
					<path
						d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.764s.784-1.764 1.75-1.764 1.75.79 1.75 1.764-.783 1.764-1.75 1.764zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z"
					/>
				</svg>
				<span>LinkedIn</span>
			</a>
			<a
				href="https://x.com/Garadiit"
				target="_blank"
				class="flex items-center space-x-2 text-zinc-400 transition-colors hover:text-white"
			>
				<svg class="h-5 w-5" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true">
					<path
						d="M18.244 2.25h3.308l-7.227 8.26 8.502 11.24H16.17l-5.214-6.817L4.99 21.75H1.68l7.73-8.835L1.254 2.25H8.08l4.713 6.231zm-1.161 17.52h1.833L7.084 4.126H5.117z"
					/>
				</svg>
				<span>Twitter</span>
			</a>
			<a
				href="https://www.credly.com/users/tegar-aditya"
				target="_blank"
				class="flex items-center space-x-2 text-zinc-400 transition-colors hover:text-white"
				aria-label="Credly Verified Badge"
			>
				<svg
					class="h-5 w-5"
					viewBox="0 0 1024 1024"
					xmlns="http://www.w3.org/2000/svg"
					fill="#000000"
					><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g
						id="SVGRepo_tracerCarrier"
						stroke-linecap="round"
						stroke-linejoin="round"
						stroke="#CCCCCC"
						stroke-width="6.144"
					></g><g id="SVGRepo_iconCarrier">
						<circle cx="512" cy="512" r="512" style="fill:#f36c21"></circle>
						<path
							d="M671.2 371.6h3c3.7.3 7.4 2.1 9.7 5 3.4 4.2 4.3 9.8 4.6 15.1.8 16.1-2.7 32.1-7.3 47.5-5.9 20.4-14.2 40-21 60.1-1.2 3.5-2.4 7.1-3.3 10.7-1.5 6-1.3 12.3-1.5 18.5-.2 5.8.2 11.6 1.3 17.3.6 3.1 1.9 6.4 4.3 8.6 2.2 2 5.4 2.9 8.3 2 3.9-1.2 7-4.2 9.8-7.1 3.9-4.3 7.6-8.7 10.3-13.8 3.8-6.8 6-14.3 7.1-22 1.5-11.6 2.7-23.4 6.9-34.4 1.6-4.2 3.6-8.5 7.4-11.1 5.1-3.6 12.8-2.1 16.7 2.7 1.9 2.4 2.4 5.5 2.4 8.4-.2 3.9-1 7.8-2.3 11.5-4.5 13.2-7.1 27.1-6.6 41.1.1 3.2.4 6.6 2.1 9.5 1.4 2.4 3.8 4.3 6.6 4.3 3.2 0 6-1.9 8-4.2 3.1-3.5 5.6-7.5 7.6-11.7 4-8.5 5.9-17.8 7.6-27 1.4-7.8 2.8-15.6 5-23.2 1.2-3.9 2.7-7.8 5.6-10.8 1.9-2.1 4.8-2.9 7.5-2.9 2.8.1 5.4 1.7 7.3 3.8 2.6 2.9 3.1 6.9 2.8 10.6-2.8 22.1-5.9 44.2-8.4 66.3-1.8 13.8-3.4 27.6-4.6 41.4-.1 1.5 1.7 2.4 2.7 1.4 7.2-6.9 14.3-14.1 19.7-22.5 2.5-3.8 4.3-7.9 6.7-11.7 1-1.7 2.2-3.4 4.1-4 2.9-1.4 6.6-1 9.1 1 1.9 1.4 2.9 3.7 3.2 6v2.7c-.6 4.6-3.3 8.5-5.3 12.5-5.5 11-13.1 21-22.6 28.9-6.8 5.8-14.8 10.2-23.2 13.2-.5.2-1.3.3-1.4 1-3.1 12.7-10 24.4-19.3 33.5-10.3 10.2-23.6 17.2-37.7 20.5-7.7 1.7-15.8 2.4-23.6 1-8-1.5-15.8-5.2-21.5-11-5.2-5.2-8.7-12.1-9.3-19.5-.6-6.7 1.1-13.5 4.3-19.4 3.7-6.7 9.3-12.3 15.9-16.2 6.3-3.8 13.5-5.6 20.6-6.5 8.1-.9 16.4-.9 24.6-.2 5.1.4 10.2.9 15.3 1.3 2.8.2 5.9 1.2 8.6-.2 1.9-.9 2.5-3.2 2.8-5.1 1.2-9 3-18.1 1.9-27.3-.2-1.2-.5-3-2-3.1-1.8.8-2.7 2.7-3.7 4.3-3.1 6-8.9 10.6-15.6 11.9-6.7 1.3-14-2.1-17.1-8.1-1.5-2.5-2.2-5.5-4.4-7.6-1.5-1.4-3.7-1.4-5.5-.6-3.2 1.4-5.3 4.3-7.9 6.5-6.8 6.1-15.4 10.7-24.7 11.2-10.8.7-21.9-5.4-26.4-15.4-.6-1.4-1.1-3.4-2.9-3.6-2-.3-3.5 1.3-4.6 2.7-5.3 6.7-10.3 13.9-17.3 18.9-4.5 3.2-9.9 5.4-15.5 5.3-5.9-.1-11.8-3.3-14.6-8.5-1.3-2.3-1.8-5.2-3.9-7-1.6-1.4-4.1-1.2-5.8-.1-2.6 1.5-4.1 4.2-6.2 6.3-5.8 5.8-14.2 8.7-22.3 7.9-9.8-1-18.7-7.8-22.3-17-.5-1.3-1.2-2.8-2.6-3.2-1.1-.4-2 .4-2.7 1.1-5.4 5-10.8 10.1-17.3 13.6-6.6 3.5-13.9 5.8-21.4 5.6-7.9.1-15.8-2.3-22.2-6.8-5.4-3.7-9.7-8.9-12.2-15-.7-1.6-1.6-3.4-3.4-3.8-1.6-.4-3 .8-3.9 2-2.7 3.8-6.2 7.1-10.1 9.6-6 3.9-13 6.6-20.3 6.6-5.6 0-11.2-2.1-15.2-6-4.3-4.2-6.6-10.1-7.5-16-1.1-7.7.5-15.5 2.7-22.8 1.4-4.8 3.2-9.4 4.3-14.3.6-2.5.8-5.2-.3-7.5-.9-1.8-2.8-2.9-4.6-3.7-2-.8-4.1.3-5.5 1.6-1.4 1.3-2.1 3-2.9 4.7-4.9 11.8-11.5 22.9-19.6 32.8-7.8 9.6-17.1 17.9-27.1 25.2-11.4 8.1-24.5 14-38.4 15.9-10.1 1.4-20.6.6-30.4-2.3-5.8-1.7-11.5-4.1-16.5-7.6-8.6-6-15.5-14.3-20.4-23.5-3.8-7.1-6.7-14.7-8.8-22.5-2.9-11.1-3.9-22.5-4.4-33.9v-7.8c.2-8.4 1-16.8 2.7-25 3-14.9 8.4-29.2 15.7-42.5 5.8-10.4 12.7-20.2 21.4-28.3 9.5-8.9 21-15.8 33.7-18.6 12.1-2.7 25.1-2 36.4 3.2 3.4 1.5 6.4 3.7 10 4.8 2.5.8 5.4.5 7.5-1.1 3.2-2.5 4.7-6.5 7.4-9.5 3.4-3.7 8.9-5.2 13.7-3.8 4.5 1.3 8 5.2 9.1 9.7.7 3 .3 6.1-.6 9-1.4 4.1-3.7 7.8-5.9 11.5-7.3 12.6-12.8 26.2-16.3 40.3-1.1 4.3-2 8.8-3.7 12.9-1.6 3.9-4.1 7.6-7.7 10-3.1 2.1-7.2 3.1-10.9 2-3.4-1-6-3.8-7.4-7-1.6-3.4-2.1-7.3-1.6-11.1 1-8.9 5.9-17 6.1-26.1.2-5.1-1.5-10.4-5.5-13.7-5.6-4.8-13.5-6.1-20.6-5.1-8.4 1.1-16.3 5.1-22.5 10.8-6.7 6.2-11.7 14-15.7 22.1-11.6 23.2-16.7 49.8-13.7 75.6 1 8.4 3 16.8 7 24.4 2.5 4.8 5.8 9.1 9.9 12.5 5.3 4.4 11.7 7.4 18.5 8.7 9.7 1.9 19.9.6 29-2.9 12.2-4.7 22.8-13.1 31.2-23 4.5-5.1 8.4-10.7 12.2-16.4 3.8-5.3 7.8-10.9 9.3-17.4 1-4.3.1-8.7-.9-12.9-.7-5.8 1.5-11.7 5.3-16 2.4-2.5 5.4-4.8 8.9-5.5 3.3-.6 7 0 9.8 2.1 3.1 2.2 4.7 6.4 3.6 10.1-.7 2.4-1.5 4.9-.8 7.4.7 2.1 2.8 3.4 4.9 3.5 4.8.4 9.8-.5 14.4 1.1 5.4 2.1 10.2 6.4 12 12.1 1.2 3.8 1.6 8.1.4 11.9-2.1 7.4-4.7 14.7-6.1 22.3-.4 2.5-.8 5.1-.1 7.6.4 1.8 2 3.4 3.9 3.5 3.3.3 6.3-1.5 8.6-3.7 4.7-4.7 7.8-10.7 10-16.9 2.7-7.5 4.1-15.4 6.1-23.1 2.1-7.9 5.3-15.6 10.3-22.1 7.4-9.8 19.4-16.1 31.8-15.8 6.9.1 13.7 2.8 18.6 7.8 4.1 4.2 6.3 9.9 7.2 15.7 1.5 9.8-.3 20.1-4.8 29-6.2 12.2-18.9 20.9-32.6 22-2 .2-4.3.1-5.8 1.6-1.3 1.3-1.2 3.3-1 5 .5 4.6 2 9.3 5.1 12.9 3.6 3.7 9 6.3 14.3 5.1 6.1-1.3 11.3-5.2 15.6-9.4 4.1-4.1 7.7-8.7 11-13.5 4.6-6.6 7.4-14.2 10.2-21.6 2.7-7.3 5.2-14.7 9.7-21.1 3.6-5.4 8.3-10.1 13.9-13.5 6.2-3.9 13.6-5.9 21-5.5 2.3.1 4.9.2 6.8-1.2 1.7-1.3 2.3-3.6 2.3-5.7 0-3.8.4-7.5.7-11.3.5-5.9 1-11.8 1.8-17.6 1.7-14.6 4.7-29 8.6-43.1 2-7.1 4.6-14.3 9.1-20.3 1.9-2.7 4.2-5.3 7.2-6.9 2.9-1.7 6.6-1.6 9.7-.7 4 1.2 6.6 5 8.2 8.6 2.9 7.1 2.1 15 1.5 22.5-.8 11.8-3.6 23.4-6 35-2.1 10.2-3.8 20.5-5.7 30.7-2.6 14-5.1 28.1-7.7 42.1-2.2 11.5-4.7 23.2-3.3 35 .4 3.1.8 6.5 2.9 8.9 1.5 1.7 4 2.1 6 1.4 2.7-.9 4.6-3.3 6-5.7 3.3-5.6 6.2-11.5 9.1-17.4 4.2-8.2 8.4-16.7 9.8-25.9 2.2-14 3.7-28.2 5.7-42.3 1.6-10.5 3.4-21 5.1-31.4 2.1-13.1 4.5-26.1 8.2-38.8 1.8-6 4.2-11.9 8.4-16.6 3.8-3.8 8.3-6.5 13.3-7zM478 487.8c-2 .6-3.6 2.2-4.9 3.8-2.9 3.7-5.1 7.9-6.6 12.4-1.6 4.8-3.1 9.8-2.5 14.8.1 1.5 1.6 2.6 3 2.6 2.7.1 5.1-1.4 7.2-3 4.7-3.3 7.7-8.4 9.8-13.6 1.3-3.3 2.2-6.9 1.9-10.5-.2-2.4-1.4-4.9-3.5-6.1-1.3-.8-3-.9-4.4-.4zm85.7 11.2c-5.6 1-10.6 4.3-14.2 8.7-3.9 4.7-6.6 10.4-8 16.4-2.1 8.5-2.3 17.5 0 26 .7 2.6 1.9 5.2 3.9 7.1 1.3 1.3 3.1 2 4.9 2.1 4.7.7 9.1-1.9 12.7-4.6 4.5-3.3 7.4-8.2 9.2-13.4 1.1-3.2.4-6.6.1-9.9-.5-6.7-.5-13.4-.1-20.1.1-2.3.8-4.5.8-6.8 0-1.8-.7-3.8-2.4-4.8-2.1-1.3-4.6-1.1-6.9-.7zm133.7 119.6c-4.8.3-9.6 1.3-14.1 3.2-4.9 2-9.1 5.7-11.2 10.5-1.4 3-2 6.6-.5 9.6 1.5 3.1 4.3 5.4 7.4 6.8 4.3 1.9 9.1 2.2 13.6 1.7 14.2-1.6 27.7-8.9 36.7-20 1.8-2.2 3.2-4.7 4.7-7.1.4-.8 1-2.1.1-2.8-1.1-.8-2.5-.5-3.7-.5-5.1-.3-10.2-.8-15.3-1-5.9-.3-11.8-.8-17.7-.4z"
							style="fill:#fff"
						></path>
					</g></svg
				>
				<span>Verified on Credly</span>
			</a>
		</div>
		<p class="text-xs">&copy; 2025 Tegar Aditya. All Rights Reserved.</p>
	</footer>
</div>
