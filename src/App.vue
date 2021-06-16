<template>
	<el-container id="app">
		<neutron-main />
	</el-container>
</template>

<script>
	import NeutronMain from './views/NeutronMain.vue';

	export default {
		name: 'App',
		components: {
			NeutronMain,
		},
	};
</script>

<style lang="scss">
	@import './assets/colours';
	@import './assets/utility';

	body {
		@include max-height;

		margin: 0;
	}

	#app {
		@include max-height;

		background: $background;
	}
</style>
