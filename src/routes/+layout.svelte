<script>
	import '../app.css';
	import { Navbar, NavBrand, NavLi, NavUl, NavHamburger } from 'flowbite-svelte';
  </script>
  
  

	<!-- Place your Navbar here to ensure it appears above the parallax background -->
	<Navbar>
	  <NavBrand href="/">
		<img src="/logo.png" class="me-3 h-6 sm:h-9" alt="Bold Logo" />
		<span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white">Onsdagsbold</span>
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
  
	<!-- Content that scrolls over the parallax background -->
		<div class="mx-auto h-800 overflow-y-scroll bg-cover bg-scroll bg-bottom bg-no-repeat shadow-lg no-scrollbar"
style="background-image:url('/background.jpg');">
	  <slot></slot> <!-- Your page content goes here -->
	</div>

  