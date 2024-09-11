<script>
	import '../app.css';
	import { Navbar, NavBrand, NavLi, NavUl, NavHamburger } from 'flowbite-svelte';
	
</script>
<style lang="postcss">
	:global(body) {
	  @apply bg-zinc-400;
	}
  </style>

<Navbar>
	<NavBrand href="/">
		<NavBrand href="/">
            <img src="/logo.png" class="me-3 h-6 sm:h-9" alt="Bold Logo" />
            <span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white">Onsdagsbold</span>
          </NavBrand>
	</NavBrand>
	<NavHamburger />
	<NavUl>
		<NavLi href="/">Home</NavLi>
		<NavLi href="/about">Apply to join</NavLi>
		<NavLi href="/contact">Player rankings</NavLi>
        <NavLi href="/contact">Next game day schedule</NavLi>
        <NavLi href="/contact">Match history and lineups</NavLi>
	</NavUl>
</Navbar>

<slot></slot>
