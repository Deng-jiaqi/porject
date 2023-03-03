<script>
	export default {
		onLaunch: function() {
			console.log('App Launch')
		},
		onShow: function() {
			console.log('App Show')
		},
		onHide: function() {
			console.log('App Hide')
		},
		globalData: {
			nums_show: [],
			nums: [],
			new_time: '',
			new_time_text: ''
		}
	}
</script>

<style lang="scss">
	@import '/commom/globel-main.css';
	@import '/commom/common.css';

	.safe-area-inset-bottom {
		padding-bottom: constant(safe-area-inset-bottom) !important;
		padding-bottom: env(safe-area-inset-bottom) !important;
	}

	/* 注意要写在第一行，同时给style标签加入lang="scss"属性 */
	@import "@/uni_modules/uview-ui/index.scss";

	.app_tiao {
		width: 100%;
		height: 16upx;
		background: #F7F7F7;
	}

	.u-tabs__wrapper__nav__item {
		flex: 1 !important;
	}

	image {
		vertical-align: top;
	}

	button::after {
		border: none;
	}

	button {
		position: relative;
		display: block;
		margin-left: auto;
		margin-right: auto;
		padding-left: 0px;
		padding-right: 0px;
		box-sizing: border-box;
		// font-size: 18px;
		text-align: center;
		text-decoration: none;
		// line-height: 1;
		line-height: 1.35;
		// border-radius: 5px;
		-webkit-tap-highlight-color: transparent;
		overflow: hidden;
		color: #000000;
		background-color: #fff;
		width: 100%;
		height: 100%;
	}

	.react {
		width: 100%;
		height: 100vh;
		display: flex;
		align-items: center;
		justify-content: center;
	}

	.bottom {
		width: 100%;
		height: 108upx;
		background: #FFFFFF;
		box-shadow: 0px -2upx 8upx 0px rgba(0, 0, 0, 0.1600);
		position: fixed;
		bottom: 0;
		padding-bottom: constant(safe-area-inset-bottom);
		padding-bottom: env(safe-area-inset-bottom);
		display: flex;
		align-items: center;
		justify-content: space-between;

		.btnH {
			margin-right: 24upx;
			display: flex;
			height: 56upx;
			border-radius: 24upx;
			overflow: hidden;
			font-size: 20upx;
			font-family: PingFangSC-Regular, PingFang SC;
			text-align: center;
			line-height: 56upx;
			font-weight: 400;
			color: #FFFFFF;

			.one {
				background: #FEA501;
				width: 162upx;
			}

			.two {
				width: 120upx;
				background: #60A496;
			}
		}

		.left {
			margin-left: 24upx;
			display: flex;
			align-items: center;

			.price {
				font-size: 26upx;
				font-family: PingFangSC-Regular, PingFang SC;
				font-weight: 400;
				color: #000000;
			}

			.times {
				font-size: 20upx;
				font-family: PingFangSC-Regular, PingFang SC;
				font-weight: 400;
				color: #000000;
			}
		}
	}
</style>
