<template>
  <main>
		<div class="shadow-lg rounded-lg bg-white p-5">
			<span>Select a currency account for your business</span>
			<div class="flex flex-col px-4 py-4">
				<!-- first-item -->
				<div class="grid grid-cols-12 py-4">
					<div class="col-span-11">
						<div class="flex">
							<img
								src="../../assets/currency-flag.png"
								alt="currency-flag"
								class="rounded-full"
								width="26"
								height="26"
							/>
							<span class="mx-4">British Account</span>
						</div>
					</div>
					<div class="col-span-1">
						<i class="fa-solid fa-plus"></i>
					</div>
				</div>
				<!-- first-item -->

				<!-- second-item -->
				<div class="grid grid-cols-12 py-4">
					<div class="col-span-11">
						<div class="flex">
							<img
								src="../../assets/currency-flag.png"
								alt="currency-flag"
								class="rounded-full"
								width="26"
								height="26"
							/>
							<span class="mx-4">British Account</span>
						</div>
					</div>
					<div class="col-span-1">
						<i class="fa-solid fa-plus"></i>
					</div>
				</div>
				<!-- second-item -->

				<!-- third-item -->
				<div class="grid grid-cols-12 py-4">
					<div class="col-span-11">
						<div class="flex">
							<img
								src="../../assets/currency-flag.png"
								alt="currency-flag"
								class="rounded-full"
								width="26"
								height="26"
							/>
							<span class="mx-4">British Account</span>
						</div>
					</div>
					<div class="col-span-1">
						<i class="fa-solid fa-plus"></i>
					</div>
				</div>
				<!-- third-item -->

				<!-- fourth-item -->
				<div class="grid grid-cols-12 py-4">
					<div class="col-span-11">
						<div class="flex">
							<img
								src="../../assets/currency-flag.png"
								alt="currency-flag"
								class="rounded-full"
								width="26"
								height="26"
							/>
							<span class="mx-4">British Account</span>
						</div>
					</div>
					<div class="col-span-1">
						<i class="fa-solid fa-plus"></i>
					</div>
				</div>
				<!-- fourth-item -->

				<!-- fifth-item -->
				<div class="grid grid-cols-12 py-4">
					<div class="col-span-11">
						<div class="flex">
							<img
								src="../../assets/currency-flag.png"
								alt="currency-flag"
								class="rounded-full"
								width="26"
								height="26"
							/>
							<span class="mx-4">British Account</span>
						</div>
					</div>
					<div class="col-span-1">
						<i class="fa-solid fa-plus"></i>
					</div>
				</div>
				<!-- fifth-item -->
				<div class="border-dashed border-t-2 my-4">
				</div>
				<div class="flex">
					<input class="bg-gray-200 p-4 outline-none rounded-md" placeholder="Name account (optional)"/>
					<div class="flex justify-end ">
						<button class="bg-blue-600 rounded-md mx-4 text-white px-3">Add account</button>
					</div>
				</div>
				
			</div>
		</div>
  </main>
</template>


<script>
	
	export default {
		name: 'Dashboard',
		components: {
			Modal,
		},
		data() {
			return {
				toggleModal: false,
			};
		},
	};
</script>

<style scoped></style>
