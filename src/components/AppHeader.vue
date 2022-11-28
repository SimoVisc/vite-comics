<script>
    import AppLogo from './AppLogo.vue';

    export default {
        name: "AppHeader",
        components:{
            AppLogo
        },
        data() {
                return {
                links: [
                    {
                    href: "#",
                    label: "CHARACTERS",
                    active: false,
                    },
                    {
                    href: "#",
                    label: "COMICS",
                    active: true,
                    },
                    {
                    href: "#",
                    label: "MOVIES",
                    active: false,
                    },
                    {
                    href: "#",
                    label: "TV",
                    active: false,
                    },
                    {
                    href: "#",
                    label: "GAMES",
                    active: false,
                    },
                    {
                    href: "#",
                    label: "COLLECTIBLES",
                    active: false,
                    },
                    {
                    href: "#",
                    label: "VIDEOS",
                    active: false,
                    },
                    {
                    href: "#",
                    label: "FANS",
                    active: false,
                    },
                    {
                    href: "#",
                    label: "NEWS",
                    active: false,
                    },
                    {
                    href: "#",
                    label: "SHOP",
                    active: false,
                    },
                ],
                };
            },
            methods: {
                changeLink(index) {
                this.links.forEach((elm, i) => {
                    if (i === index) {
                    elm.active = true;
                    } else {
                    elm.active = false;
                    }
                });
            },
        },
    };
</script>
 
<template>
  <header class="container">
     <AppLogo/>
     <nav class="main-nav">
            <ul>
                <li v-for=" (item,index) in links">
                    <a 
                    :class="{active: item.active}" 
                    :href= "item.href" 
                    @click.prevent="changeLink(index)"
                    >{{item.label}}</a>
                </li>
            </ul>
      </nav>
  </header>
</template>

<style lang="scss" scoped>
 header{
    display: flex;
    justify-content: space-between;
    align-items: center;
    text-align: center;
    padding-top: 10px;

    .main-nav {
        ul {
            display: flex;
            list-style: none;
            a{
            display: inline-block;
            margin: 10px;
            padding: 40px 0;
            font-size: 80%;
            color:#000;
            text-decoration: none;
            &.active{
                border-bottom: var(--primary-color) solid 4px ;
            }
           }
        }
    }
 }
</style>