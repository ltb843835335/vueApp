<template>
    <div>
        <home-header></home-header>
        <home-swiper></home-swiper>
    </div>
</template>

<script>
import HomeHeader from './Header'
import HomeSwiper from './Swiper'
export default {
    name : 'Home',
    components:{
        HomeHeader,
        HomeSwiper
    }
}
</script>

<style>

</style>
