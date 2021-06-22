<template>
	<el-container id="app">
		<side-menu />
		<neutron-main />
	</el-container>
</template>

<script>
	import NeutronMain from './views/NeutronMain.vue';
	import SideMenu from './components/SideMenu.vue';

	export default {
		name: 'App',
		components: {
			SideMenu,
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
