<template>
	<div v-if="toggleModal">
		<div class="fixed z-40 inset-0 opacity-25 bg-black"></div>
		<div
			class="fixed overflow-x-hidden inset-0 flex justify-center items-center z-50"
		>
			<div class="flex flex-col rounded-lg shadow-lg bg-white">
				<div class="p-5">
					<div class="flex justify-between items-start">
						<slot name="title"></slot>
						<button @click="$emit('close')">
							<i class="fa-solid fa-xmark"></i>
						</button>
					</div>
				</div>
				<div class="p-6">
					<slot></slot> 
				</div>
			</div>
		</div>
	</div>
</template>

<script>
	export default {
		name: 'Modal',
		data() {
			return {};
		},
		props: ['toggleModal'],
		
	};
</script>
