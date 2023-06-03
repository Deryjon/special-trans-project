<template>
  <div class="header-menu ml-[90px]">
    <ul class="menu flex">
      <li class="mr-14 hover:text-brand cursor-pointer duration-300"
			v-for="(item, idx) in menuItems" 
			:key="item"
			>{{item.name}}</li>
      
    </ul>
  </div>
</template>
<script>
	import menuList from '../meniList'
export default {
	data() {
		return{
			menuItems: menuList
		}
	}
}
</script>
