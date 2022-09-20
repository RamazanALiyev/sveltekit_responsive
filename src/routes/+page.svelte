<script>
	import image from '../routes/assets/Group.svg';
	import model1 from '../routes/assets/Group (2).svg';
	import model2 from '../routes/assets/XMLID_1_ (1).svg';
	import model3 from '../routes/assets/XMLID_1_ (2).svg';
	import model4 from '../routes/assets/XMLID_1_.svg';
	import model5 from '../routes/assets/XMLID_24_.svg';
	import women from '../routes/assets/picwomen.svg';
	import men from '../routes/assets/picmen.svg';
	import talantsman from '../routes/assets/talanstman.svg';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section class="bg-emerald-400">
	<div
		class="w-[95%] pt-7 mx-auto flex flex-col items-center md:w-[90%] md:flex-row-reverse md:justify-between md:items-center"
	>
		<div class="flex justify-center items-center md:w-3/5">
			<img class="w-11/12" src={image} alt="pic" />
		</div>
		<div class="mt-7 md:w-2/6">
			<h3 class="workSans font-bold text-base uppercase text-white">Welcome</h3>
			<h5 class="crimsonText font-bold text-[28px] text-white my-[15px] md:text-[40px]">
				Lorem ipsum dolor sit amet consectetur
			</h5>
			<p class="workSans font-normal text-[15px] text-white">
				Lorem ipsum, dolor sit amet consectetur adipisicing elit. Suscipit nemo hic quos, ab, dolor
				aperiam nobis cum est eos error ipsum, voluptate culpa nesciunt delectus iste?
			</p>
			<button class="workSans text-xl px-[47px] py-[10px] bg-white rounded-[5px] mt-6 mb-10"
				>Explore</button
			>
		</div>
	</div>
</section>

<section class="py-6 mx-auto flex flex-col items-center">
	<div>
		<h3 class="workSans text-emerald-600 uppercase font-bold text-base text-center">partners</h3>
		<h1 class="crimsonText text-2xl font-bold text-black text-center my-4">Lorem Ipsum Dolor</h1>
		<p class="workSans text-[20px] text-center">
			Lorem ipsum, dolor sit amet consectetur adipisicing elit.
		</p>
	</div>
	<div class="flex w-[80%] items-center justify-center flex-col my-10 md:flex-row">
		<img class="my-2 mx-4 w-[150px]" src={model1} alt="model" />
		<img class="my-2 mx-4 w-[150px]" src={model2} alt="model" />
		<img class="my-2 mx-4 w-[150px]" src={model3} alt="model" />
		<img class="my-2 mx-4 w-[150px]" src={model4} alt="model" />
		<img class="my-2 mx-4 w-[150px]" src={model5} alt="model" />
	</div>
	<button
		class="workSans text-xl px-[47px] bg-gray-900 text-white rounded-[5px] px-[30px] py-[13px]"
		>Learn More</button
	>
</section>

<section class="py-5">
	<div class="w-[95%] mx-auto my-5 md:flex md:items-center md:w-[90%]">
		<div class="flex justify-center items-center w-full">
			<img src={women} alt="" />
		</div>
		<div class="py-10">
			<h2 class="crimsonText text-gray-900 font-bold text-2xl">
				Lorem ipsum dolor sit amet consectetur
			</h2>
			<p class="workSans text-[15px] text-gray-600 my-5">
				Lorem ipsum, dolor sit amet consectetur adipisicing elit. Suscipit nemo hic quos, ab, dolor
				aperiam nobis cum est eos error ipsum, voluptate culpa nesciunt delectus iste?
			</p>
			<button
				class="workSans text-xl px-[47px] bg-gray-900 text-white rounded-[5px] px-[30px] py-[13px]"
				>Learn More</button
			>
		</div>
	</div>
	<div class="w-[95%] mx-auto my-5 md:flex md:items-center md:flex-row-reverse md:w-[90%]">
		<div class="flex justify-center items-center w-full">
			<img src={men} alt="" />
		</div>
		<div class="py-10">
			<h2 class="crimsonText text-gray-900 font-bold text-2xl">
				Lorem ipsum dolor sit amet consectetur
			</h2>
			<p class="workSans text-[15px] text-gray-600 my-5">
				Lorem ipsum, dolor sit amet consectetur adipisicing elit. Suscipit nemo hic quos, ab, dolor
				aperiam nobis cum est eos error ipsum, voluptate culpa nesciunt delectus iste?
			</p>
			<button
				class="workSans text-xl px-[47px] bg-gray-900 text-white rounded-[5px] px-[30px] py-[13px]"
				>Learn More</button
			>
		</div>
	</div>
</section>

<section class="flex flex-col items-center py-8">
	<div>
		<h3 class="workSans text-emerald-600 uppercase font-bold text-base text-center">team</h3>
		<h1 class="crimsonText text-2xl font-bold text-black text-center my-4">Our Talents</h1>
		<p class="workSans text-[20px] text-center">
			Lorem ipsum, dolor sit amet consectetur adipisicing elit.
		</p>
	</div>
	<div class="w-full">
		<div class="mx-auto flex flex-col gap-8 my-8 md:flex-row md:w-[90%]">
			<div class="shadow border w-3/4 mx-auto py-5 px-10">
				<img class="mx-auto" src={talantsman} alt="" />
				<h3 class="crimsonText font-bold text-gray-900 text-2xl my-3">Peg Legge</h3>
				<span class="workSans text-[15px] text-gray-600">CEO</span>
			</div>
			<div class="shadow border w-3/4 mx-auto py-5 px-10">
				<img class="mx-auto" src={talantsman} alt="" />
				<h3 class="crimsonText font-bold text-gray-900 text-2xl my-3">Peg Legge</h3>
				<span class="workSans text-[15px] text-gray-600">CEO</span>
			</div>
			<div class="shadow border w-3/4 mx-auto py-5 px-10">
				<img class="mx-auto" src={talantsman} alt="" />
				<h3 class="crimsonText font-bold text-gray-900 text-2xl my-3">Peg Legge</h3>
				<span class="workSans text-[15px] text-gray-600">CEO</span>
			</div>
			<div class="shadow border w-3/4 mx-auto py-5 px-10">
				<img class="mx-auto" src={talantsman} alt="" />
				<h3 class="crimsonText font-bold text-gray-900 text-2xl my-3">Peg Legge</h3>
				<span class="workSans text-[15px] text-gray-600">CEO</span>
			</div>
		</div>
	</div>
	<button
		class="workSans text-xl px-[47px] bg-gray-900 text-white rounded-[5px] px-[30px] py-[13px]"
		>Learn More</button
	>
</section>

<style>
	@import url('https://fonts.googleapis.com/css2?family=Work+Sans:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
	@import url('https://fonts.googleapis.com/css2?family=Crimson+Text:ital,wght@0,400;0,600;0,700;1,400;1,600;1,700&display=swap');
	h3.workSans,
	p.workSans,
	button.workSans {
		font-family: 'Work Sans', sans-serif;
	}
	h3.workSans {
		letter-spacing: 5px;
	}
	h5.crimsonText {
		font-family: 'Crimson Text', serif;
	}
	div.shadow {
		box-shadow: 3px 4px 12px 1px rgba(0, 0, 0, 0.25);
		border-radius: 5px;
	}
</style>
