<script>
	import image from '../routes/assets/Group.svg';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section class="bg-emerald-400">
	<div class="w-[95%] pt-7 mx-auto flex flex-col items-center md:w-[90%] md:flex-row-reverse md:justify-between md:items-center">
		<div class="flex justify-center items-center md:w-3/5"><img class="w-11/12" src={image} alt="pic" /></div>
		<div class="mt-7 md:w-2/6">
			<h3 class="workSans font-bold text-base uppercase text-white">Welcome</h3>
			<h5 class="crimsonText font-bold text-[28px] text-white my-[15px] md:text-[40px]">Lorem ipsum dolor sit amet consectetur</h5>
			<p class="workSans font-normal text-[15px] text-white">
				Lorem ipsum, dolor sit amet consectetur adipisicing elit. Suscipit nemo hic quos, ab, dolor
				aperiam nobis cum est eos error ipsum, voluptate culpa nesciunt delectus iste?
			</p>
			<button class="workSans text-xl px-[47px] py-[10px] bg-white rounded-[5px] mt-6 mb-10">Explore</button>
		</div>
	</div>
</section>


<style>
	@import url('https://fonts.googleapis.com/css2?family=Work+Sans:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
	@import url('https://fonts.googleapis.com/css2?family=Crimson+Text:ital,wght@0,400;0,600;0,700;1,400;1,600;1,700&display=swap');
	h3.workSans,
	p.workSans,
	button.workSans {
		font-family: 'Work Sans', sans-serif;
	}
	h3.workSans{
		letter-spacing: 5px;
	}
	h5.crimsonText {
		font-family: 'Crimson Text', serif;
	}
</style>
