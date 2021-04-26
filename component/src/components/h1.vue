<template>
	<div id="message">
		<h1>{{msg}}</h1>
	</div>
</template>

<script>
export default {
	name: 'MESSAGE',
	props: {
	msg: String
	}
}
</script>

<style>
	.message{
		color: #42B983;
	}
</style>
