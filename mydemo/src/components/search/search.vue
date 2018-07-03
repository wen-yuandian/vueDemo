<template>
	<div class="box">
		<div class="search">
			这里是搜索页面
			<div class="search2">
				这是子集块
			</div>
		</div>
		<div class="search2">
			这是第二个块
		</div>
		<div>{{a}}</div>
		<p></p>
		<div class="math">{{math}}</div>
		
		
		<div @click="fn">方法之后</div>
	</div>
</template>

<script>
	export default {
		data(){
			return {
				a:1,
				b:2
			}
		},

		computed:{
			math() {
				
					return this.a+this.b
				
			}
		},
		methods:{
			fn(){
			 this.a=this.a+3
			}
		},
		watch:{
			// a(val){
			// 	return this.a+10
			// }
		}
	}
</script>

<style lang="stylus">
	.box
		.search 
			background red
			color white
			pad(10px,15px)
			.search2
				font-size 32px
				&:hover
					color yellow
		
</style>
