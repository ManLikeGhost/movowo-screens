<template>
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
        <div class="flex flex-col ml-3 mb-52">
          <span>Accounts</span>
          <span>Transactions</span>
          <span>Cards</span>
          <span>Settings</span>
        </div>
        <div class="flex flex-col ml-3">
          <span>Help & support</span>
          <spanp>Logout</spanp>
        </div>
			</div>
		</div>
		<div class="col-span-10">
			<div class="pl-16 pr-8 mt-10">
				<div class="flex justify-between">
					<div>
						<div class="mb-16">
							<h3 class="text-3xl">Accounts</h3>
							<p>Accounts Overview</p>
						</div>
						<div class="flex mb-14">
							<button class="bg-gray-200 rounded-md p-2">Send Funds</button>
							<button class="bg-gray-200 rounded-md p-2 mx-2">Add Funds</button>
							<button class="bg-gray-200 rounded-md p-2 mr-2">Exchange</button>
							<button class="bg-gray-200 rounded-md p-2">Add Account</button>
						</div>
            <div>
              <p>All accounts</p>
							<div class="rounded p-4 border">
								<div class="flex justify-between mb-8">
									<span>Main</span>
									<span>icon</span>
								</div>
								<div>
									<h2>#0.00</h2>
									<span>view account details</span>
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
	export default {
		name: 'Dashboard',
	};
</script>

<style scoped></style>
