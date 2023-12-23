<script lang="ts">
	import '../app.postcss';

	function visitG(){
		window.open('https://github.com/BenFletcher0','_blank');
	}
	function visitL(){
		window.open('https://www.linkedin.com/in/ben-fletcher-/','_blank')
	}

</script>

<!--nav bar for the different routes-->
<title>Portfolio Website</title>

<nav>
	<a href = "../">Home</a>
	<a href = "../About">About</a>
	<a href = "../Projects">Projects</a>
</nav>


<!--any page using this layout will be inserted in this slot-->
<slot />


<!-- A footer with clickable links to socials-->
	<nav>
		<button type = "submit" class="btn" on:click={visitG}>
			<img class = "rounded-full w-10 h-10"src = "github.png" alt = "Github"/>
		</button>
		<button class="btn" on:click={visitL}>
			<img class = "rounded-full w-10 h-10" src = "linkedin.png" alt = "LinkedIn" />
		</button>
	</nav>

