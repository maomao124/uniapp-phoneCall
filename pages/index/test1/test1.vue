<template>
	<view>
		<button type="primary" @click="call('1234567')">拨打电话1234567</button>
		<button type='warn' @click="call('110')">拨打电话110</button>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				
			}
		},
		methods: {
			call(number)
			{
				uni.makePhoneCall({
					phoneNumber: number
				})
			}
		}
	}
</script>

<style>

</style>
