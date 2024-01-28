<template>
	<!-- wrap, container를 만드는이유 : 가장 바깥쪽 레이아웃의 큰 틀을 만들어주는 작업이다. -->
  <div class="wrap">
		<div class="container">
			<MainView />
		</div>
	</div>
</template>

<script>
import MainView from '../components/MainView.vue'
export default {
  components: { MainView },

}
</script>

<style lang="scss" scoped>
	@import '../scss/main.scss';

	.wrap {
		@include center;
		width: 100%;
		height: 100vh;
		font-size: 16px;

		.container {
			@include center-sb;
			width: 55%;
			height: 90%;
			max-width: 1920px;
			max-height: 1354px;
		}
	}
</style>