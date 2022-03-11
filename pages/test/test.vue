<template>
	<view>
			test page
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		beforeCreate(){
			console.log("test beforeCreate")
		},
		created() {
			console.log("test created")
		},
		beforeMount() {
			console.log("test beforeMount")
		},
		mounted() {
			console.log("test mounted")
		},
		beforeDestroy() {
			console.log("test beforeDestroy")
		},
		destroyed() {
			console.log("test destroyed")
		},
		onLoad(e) {
			console.log(e);
			console.log("index load")
		},
		onHide(){
			console.log("test hide");
		},
		onUnload() {
			console.log("test unload")
		},
		methods: {
			
		}
	}
</script>

<style>

</style>
