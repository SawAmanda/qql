<template>
    <div class="container">
        <Header></Header>
        <Banner></Banner>
        <Mainbusiness></Mainbusiness>
        <Mainadvantage></Mainadvantage>
        <Techicalteam></Techicalteam>
        <Power></Power>
        <Platform></Platform>
        <Media></Media>
        <Footer></Footer>
    </div>
</template>

<script>
import Header from './common/Header'
import Banner from './home/Banner'
import Mainbusiness from './home/Mainbusiness'
import Mainadvantage from './home/Mainadvantage'
import Techicalteam from './home/Techicalteam'
import Power from './home/Power'
import Platform from './home/Platform'
import Media from './home/Media'
import Footer from './common/Footer'
export default {
    components: {
        Header,
        Banner,
        Mainbusiness,
        Mainadvantage,
        Techicalteam,
        Platform,
        Power,
        Media,
        Footer
    }
}
</script>

<style>

</style>
