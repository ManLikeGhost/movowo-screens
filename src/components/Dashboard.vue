<template>
	<Modal :toggleModal="toggleModal" @close="toggleModal = false">
		<template v-slot:title> Add account </template>
		<AddAccount/>
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
	</div>
</template>

<script>
	import Modal from './utilities/Modal.vue';
	import AddAccount from './layout/AddAccount.vue'
	export default {
		name: 'Dashboard',
		components: {
			Modal,
			AddAccount
		},
		data() {
			return {
				toggleModal: false,
			};
		},
	};
</script>

<style scoped></style>
