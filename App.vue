<script>
	export default {
		globalData: {
			globalText: 'globalText'
		},
		onLaunch: function() {
			console.log('App Launch')
		},
		onShow: function() {
			console.log('App Show')
		},
		onHide: function() {
			console.log('App Hide')
		}
	}
</script>

<style>
	/* #ifdef H5 */
	@import "vant/lib/index.css"
	/* #endif */
	/* #ifdef MP */
	@import "/wxcomponents/vant/dist/common/index.wxss"
	/* #endif */
	/*每个页面公共css */
</style>
