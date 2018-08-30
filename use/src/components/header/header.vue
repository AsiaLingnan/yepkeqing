<template>
	<h1 v-if="!this.$route.query.tittle">{{msg}}</h1><!-- 默认值 -->
	<h1 v-else>{{this.$route.query.tittle}}</h1>
</template>

<script>
	export default{
	    data () {
	      return {
	        msg: '首页'
	      }
	    }
	}
</script>

<style scoped="">
	body{
		width:100%;
		margin: 0px;
		padding: 0px;
	}
	h1{
		width: 100%;
		margin: 0px;
		padding:5px 0px 10px 0px;
		color: #fff;
		text-align: center;
		box-shadow:0px 3px  3px 1px #eef;
		background: orange;
		position: fixed;
		top: 0px;
		left: 0px;
		z-index: 10;
		font-size:18px;	
	}
	
</style>