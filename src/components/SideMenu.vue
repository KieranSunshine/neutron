<template>
	<el-menu background-color="#393E46" collapse="false">
		<el-menu-item index="1" >
			<i class="el-icon-position" />
			<template #title>Requests</template>
		</el-menu-item>
		<el-menu-item index="2">
			<i class="el-icon-takeaway-box" />
			<template #title>History</template>
		</el-menu-item>

		<!-- Something spooky is happening with this one -->
		<!-- Looks like the width is going dodgy of the hover div. -->
		<el-menu-item index="4" class="weighted-menu-item">
			<i class="el-icon-setting" />
			<template #title>Settings</template>
		</el-menu-item>
	</el-menu>
</template>

<script lang="ts">
	import { defineComponent } from 'vue';

	export default defineComponent({
		name: 'SideMenu',
		data() {
			return {
				isCollapsed: false,
			};
		},
		methods: {
		},
	});
</script>

<style lang="scss" scoped>
	.weighted-menu-item {
		position: absolute;
		bottom: 0;
	}
</style>
