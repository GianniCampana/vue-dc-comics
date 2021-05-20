<template>

<header>
    <div class="header-logo">
        <img src="../assets/img/dc-logo.png" alt="">
    </div>
    <div class="header-menu">
        <ul>
            <li  v-for="(link,index) in links" :key="index">
                <a :class="{'active': link.current}" href="link.url">{{link.text}}</a>
            </li>
        </ul>
    </div>
</header>
    
</template>


<script>
export default {
    name: 'Header',
    data(){
    return{

        links: [
            {
                text: 'HOME',
                url: '#',
                current: false
            },
            {
                text: 'COMICS',
                url: '#',
                current: false
            },
            {
                text: 'MOVIES',
                url: '#',
                current: false
            },
            {
                text: 'TV',
                url: '#',
                current: false
            },
            {
                text: 'GAMES',
                url: '#',
                current: false
            },
            {
                text: 'COLLECTIBLES',
                url: '#',
                current: false
            },
            {
                text: 'VIDEOS',
                url: '#',
                current: false
            },
            {
                text: 'FUNS',
                url: '#',
                current: false
            },
            {
                text: 'NEWS',
                url: '#',
                current: false
            },
            {
                text: 'SHOP',
                url: '#',
                current: false
            }
        ]
        
    }
}
}

</script>

<style lang='scss'>



header{
    height: 100px;
    display: flex;
    .header-menu{
        
        height: 100px;
        
        ul{
            height: 100px;
            list-style: none;
            display: flex;
            li{
                height: 100px;
                margin-left: 20px;
                }
            li a{
                height: 100px;
                display: flex;
                align-items: center;
                font-family: 'Raleway', sans-serif;
                font-weight: 500;
                cursor: pointer;
                text-decoration: none;
                color: black;
                &:hover,
                &.active{
                border-bottom: blue 5px solid;
                 }
                
               
            }
        }
    }
}

.header-logo{
    height: 100px;
    
    width: 30%;
    img{
        margin-left: 250px;
        margin-top: 10px;
        width: 80px;
    }
    
}

</style>
