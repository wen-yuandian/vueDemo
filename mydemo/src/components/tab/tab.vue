<template>
	<div id="tab">
		<router-link tag="div" to="/recommend" class="tab-item">
			<span>推荐</span>
		</router-link>
		<router-link tag="div" to="/singer" class="tab-item">
			<span>歌手</span>
		</router-link>
		<router-link tag="div" to="/rank" class="tab-item">
			<span>排行榜</span>
		</router-link>
		<router-link tag="div" to="/search" class="tab-item">
			<span>搜索</span>
		</router-link>
	</div>
</template>

<script>
export default {

}
</script>

<style>

#tab {
	display: flex;
	width: 300px;
}
#tab .tab-item {
	flex: 1 1 0%;
	line-height: 25px;
	background: #333;
	color: #fff;
}
#tab .tab-item:nth-of-type(1) {
	flex: 1 2 100px;
}
#tab .tab-item:nth-of-type(2) {
	flex: 1 1 100px;
}
#tab .tab-item:nth-of-type(3) {
	flex: 1 1 100px;
}
#tab .tab-item:nth-of-type(4) {
	flex: 1 1 100px;
}
</style>