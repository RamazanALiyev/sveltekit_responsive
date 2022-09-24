<script>
	let regex = /^[A-Za-z0-9_!#$%&'*+\/=?`{|}~^.-]+@[A-Za-z0-9.-]+$/gm;
	const fields = { name: '', email: '', message: '' };
	const errors = { name: '', email: '', message: '' };
	let valid = false;
	const submitHandler = () => {
		valid = true;
		if (fields.name.trim().length < 5) {
			valid = false;
			errors.name = 'Name must be at least 5 characters long';
		} else {
			errors.name = '';
		}

		if (!fields.email.match(regex)) {
			valid = false;
			errors.email = 'Email cannot match in email rulers';
		} else {
			errors.email = '';
		}

		if (valid) {
			localStorage.setItem('fields', JSON.stringify(fields));
			fields.name = '';
			fields.email = '';
			fields.message = '';
		}
	};
</script>

<form class="md:w-1/2" on:submit|preventDefault={submitHandler}>
	<div class="flex flex-col">
		<label class="workSans text-xl my-4" for="name">Name</label>
		<input
			class="border border-gray-800 outline-none pl-2 w-full h-[40px] md:w-[95%]"
			id="name"
			type="text"
			bind:value={fields.name}
		/>
		<div class="text-red-900 text-xs font-bold tracking-widest mt-2 rounded-md">{errors.name}</div>
	</div>
	<div class="flex flex-col">
		<label class="workSans text-xl my-4 md:my-1" for="email">Email</label>
		<input
			class="border border-gray-800 outline-none pl-2 w-full h-[40px] md:w-[95%]"
			id="email"
			type="text"
			bind:value={fields.email}
		/>
		<div class="text-red-900 text-xs font-bold tracking-widest mt-2 rounded-md">{errors.email}</div>
	</div>
	<div class="flex flex-col">
		<label class="workSans text-xl my-4" for="message">Message</label>
		<textarea
			class="border border-gray-800 outline-none pl-2 w-full h-[140px] md:w-[95%]"
			id="message"
			bind:value={fields.message}
		/>
	</div>
	<button
		class="h-[40px] bg-black text-white mt-8 rounded-md w-full md:w-[95%] md:mt-3"
		type="submit">Submit</button
	>
</form>

<style>
	@import url('https://fonts.googleapis.com/css2?family=Work+Sans:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
	@import url('https://fonts.googleapis.com/css2?family=Crimson+Text:ital,wght@0,400;0,600;0,700;1,400;1,600;1,700&display=swap');
	label.workSans {
		font-family: 'Work Sans', sans-serif;
	}
</style>
