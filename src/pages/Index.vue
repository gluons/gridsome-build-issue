<template>
	<Layout>
		<div id="radio-btns">
			<RadioToggleButtons
				v-model='currentValue'
				:values='values'
				color='purple'
			/>
		</div>
	</Layout>
</template>

<script>
const values = [...Array(5).keys()].map(i => ({
	label: `Value ${i + 1}`,
	value: `${i + 1}`
}));

export default {
	data() {
		return {
			currentValue: '1',
			values
		};
	},
	metaInfo: {
		title: 'Hello, world!'
	}
}
</script>

<style>
#radio-btns {
	margin-top: 10%;
	display: flex;
	justify-content: center;
}
</style>
