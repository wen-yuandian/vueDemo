<!--推荐页面 -->
<template>
	<div class="box">
		<ul>
			<li v-for="item in list" :key="item.cur_count">{{item.data.albumname}}</li>
		</ul>
	</div>
</template>

<script>
    import mydata from '@/api/api'
	export default {
		data(){
			return {
				list:mydata.a.songlist
			}
		}
	}
	console.log(mydata)
</script>

<style>
.box {
	text-align: left;
}
li {
	padding-left: 5px;
	border-bottom: 1px solid #bbb;
	line-height: 24px;
}
</style>