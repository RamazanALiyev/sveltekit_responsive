<script>
	import map from '../assets/map.svg';
	import Form from '../../components/Form.svelte';
</script>

<div class="py-12">
	<div class="pb-9">
		<h1 class="crimsonText font-bold text-2xl text-center mb-4">Contact Us</h1>
		<p class="workSans text-xl text-center leading-8">
			Lorem ipsum, dolor sit amet consectetur adipisicing elit.
		</p>
	</div>
	<div class="w-[95%] mx-auto md:w-[90%] md:flex md:flex-row-reverse">
		<div class="map mb-5 md:mb-0 md:w-1/2">
			<img class="w-full md:h-full md:object-cover" src={map} alt="pic" />
		</div>
		<Form />
	</div>
</div>

<style>
	@import url('https://fonts.googleapis.com/css2?family=Work+Sans:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
	@import url('https://fonts.googleapis.com/css2?family=Crimson+Text:ital,wght@0,400;0,600;0,700;1,400;1,600;1,700&display=swap');
	h1.crimsonText {
		font-family: 'Crimson Text', serif;
	}
	p.workSans {
		font-family: 'Work Sans', sans-serif;
	}
</style>
