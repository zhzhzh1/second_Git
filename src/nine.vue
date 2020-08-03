<template>
	<div id="main">
		<div class="row" v-for="c in color">
			
			<div class="column" v-for="d in div" >
				
				{{d.name}}
			</div>
		</div>
	</div>
</template>

<script>
	export default{
		name:'nine',
	data(){
		return{
			color:[
				{type:'white','index':1},
				{'type':'black','index':2},
				{'type':'red','index':3},
				{'type':'green',/*  */'index':4}
			],
			div:[
				{'name':'1','index':1},
				{'name':'2','index':2},
				{'name':'3','index':3},
				{'name':'4','index':4},
			],
			
		}
	}
	}
</script>

<style>
	.row{
		width: 50px;
		height: 50px;
		float: left;
		border: 1px solid black;
		
	}
	.column{
		width: 50px;
		height: 50px;
		border: 1px solid black;
	}
	#main{
		height: 400px;
		width: 500px;
		border:1px solid
	}
</style>

//v-model:双向数据绑定原理2.x与3.x不同
//2.x是属性监听propertyListener