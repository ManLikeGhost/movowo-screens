<template>
  <div class='container mx-auto'>
    <Dashboard/>
    
  <router-view />
  </div>
</template>

<script>
	import Dashboard from '@/components/Dashboard';
	export default {
		components: { Dashboard },
	};
</script>

<style>
	
</style>
