<template>
	<view>
		<EpInput :disabled="false" v-model="select" :options="list" @change="change"></EpInput>
	</view>
</template>

<script>
	import EpInput from "./components/EpInput.vue"
	export default{
		components:{
			EpInput
		},
		data(){
			return {
				list: [
					 {value:"1",label: 'test1'},
					 {value:"2",label: 'test2'},
					 {value:"3",label: 'test3'},
					 {value:"4",label: 'test4'},
					 {value:"5",label: 'test5'},
					 {value:"6",label: 'test6'},
					 {value:"7",label: 'test7'}
				],
				select: ''
			}
		},
		methods:{
			change(e){
				console.log('select = ',this.select)
			},
		}
		
	}
</script>

<style>
</style>