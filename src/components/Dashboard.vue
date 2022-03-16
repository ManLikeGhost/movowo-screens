<template>
	<Modal :toggleModal="toggleModal" @close="toggleModal = false">
		<template v-slot:title> Add account </template>
		<div class="shadow-lg rounded-lg bg-white p-5">
			<span>Select a currency account for your business</span>
			<div class="flex flex-col px-4 py-4">
				<!-- first-item -->
				<div class="grid grid-cols-12 py-4">
					<div class="col-span-11">
						<div class="flex">
							<img
								src="../assets/currency-flag.png"
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
								src="../assets/currency-flag.png"
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
								src="../assets/currency-flag.png"
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
								src="../assets/currency-flag.png"
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
								src="../assets/currency-flag.png"
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
	</Modal>
	<div class="grid grid-cols-12">
		<div class="col-span-2 bg-gray-200 h-screen">
			<div class="mt-4">
				<div class="flex justify-evenly mb-48">
					<div class="rounded-full bg-gray-300 mt-2">
						<div class="text-3xl m-4">D</div>
					</div>
					<div class="mt-4">
						<span>David Omomia</span>
						<p>AduniTech LTD</p>
					</div>
					<div class="text-2xl mt-8">+</div>
				</div>
				<div class="flex flex-col gap-4 content-between ml-3 mb-40">
					<span>Accounts</span>
					<span>Transactions</span>
					<span>Cards</span>
					<span>Settings</span>
				</div>
				<div class="flex flex-col gap-2 content-between ml-3">
					<span>Help & support</span>
					<span>Logout</span>
				</div>
			</div>
		</div>
		<div class="col-span-10 bg-slate-50">
			<div class="pl-16 pr-8 mt-10">
				<div class="flex justify-between">
					<div>
						<div class="mb-16">
							<h3 class="text-3xl">Accounts</h3>
							<p>Accounts Overview</p>
						</div>
						<div class="flex mb-14">
							<button class="bg-gray-200 rounded-md p-2 hover:bg-gray-400">
								Send Funds
							</button>
							<button class="bg-gray-200 rounded-md p-2 mx-2 hover:bg-gray-400">
								Add Funds
							</button>
							<button class="bg-gray-200 rounded-md p-2 mr-2 hover:bg-gray-400">
								Exchange
							</button>
							<button
								class="bg-gray-200 rounded-md p-2 hover:bg-gray-400"
								@click="toggleModal = !toggleModal"
							>
								Add Account
							</button>
						</div>
						<div>
							<p class="mb-2">All accounts</p>
							<div class="rounded-lg p-4 bg-white shadow-md">
								<div class="flex justify-between mb-8">
									<div>
										<span>Main</span>
										<p class="font-light">NGN</p>
									</div>
									<img
										src="../assets/currency-flag.png"
										alt="currency-flag"
										class="rounded-full"
									/>
								</div>
								<div>
									<h1 class="text-2xl font-normal">#0.00</h1>
									<div class="flex">
										<span class="text-blue-600">view account details</span>
										<i
											class="fa-solid fa-arrow-right pt-1 pl-2 text-blue-600"
										></i>
									</div>
								</div>
							</div>
						</div>
					</div>
					<div>
						<span>icon</span>
					</div>
				</div>
			</div>
		</div>
		<!-- copied-stuff -->
		<!-- <div
		class="fixed overflow-x-hidden overflow-y-auto inset-0 flex justify-center items-center z-50"
		v-if="toggleModal"
	>
		<div class="relative mx-auto w-auto max-w-2xl">
			<div class="bg-white rounded px-6 py-6">
				<div class="flex justify-between mb-4">
					<div><h1>Add Account</h1></div>
					<div><span @click="toggleModal = !toggleModal">X</span></div>
				</div>
				<div class="rounded bg-slate-50">
					<span class="text-gray-700 px-2"
						>select a currency account for your business</span
					>
				</div>
				<div></div>
			</div>
		</div>
	</div>
	<div
		v-if="toggleModal"
		class="absolute z-40 inset-0 opacity-25 bg-slate-500"
	></div> -->
		<!-- copied-stuff -->
	</div>
</template>

<script>
	import Modal from './utilities/Modal.vue';
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
