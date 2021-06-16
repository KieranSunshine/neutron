<template>
	<el-main id="main">
		<el-row id="main_row">
			<!-- Need to implement a multi-pane to make these resizeable -->
			<!-- Consisting of a multipane component with multipane-separators dividing the content-->
			<el-col :span="8" class="bordered-column">
				<request-history />
			</el-col>
			<el-col :span="8" class="bordered-column">

			</el-col>
			<el-col :span="8">

			</el-col>
		</el-row>
	</el-main>
</template>

<script>
	import RequestHistory from '../components/RequestHistory.vue';

	export default {
		name: 'NeutronMain',
		components: {
			RequestHistory,
		},
	};
</script>

<style lang="scss" scoped>
	@import '../assets/utility';

	#main {
		@include no-padding;
	}

	#main_row {
		@include max-height;
	}

	.bordered-column {
		border-style: solid;
		border-width: 0 1px 0 0;
	}

</style>
