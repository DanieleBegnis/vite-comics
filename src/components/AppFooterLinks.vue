<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            comics: [
                {
                    text: 'Characters',
                },
                {
                    text: 'Comics',
                },
                {
                    text: 'Movies',
                },
                {
                    text: 'TV',
                },
                {
                    text: 'Games',
                },
                {
                    text: 'Videos',
                },
                {
                    text: 'News',
                }
            ],
            shop: [
                {
                    text: 'Shop DC'
                },
                {
                    text: 'Shop DC Collectibles'
                }
            ],
            dc: [
                {
                    text: 'Terms of use',
                },
                {
                    text: 'Privacy policy',
                },
                {
                    text: 'Ad choices',
                },
                {
                    text: 'Advertising',
                },
                {
                    text: 'Jobs',
                },
                {
                    text: 'Subscription',
                },
                {
                    text: 'Talent workshop',
                },
                {
                    text: 'CPSC certificate',
                },
                {
                    text: 'Ratings',
                },
                {
                    text: 'Shop help',
                },
                {
                    text: 'Contact us',
                }
            ],
            sites: [
                {
                    text: 'DC',
                },
                {
                    text: 'MAD magazine',
                },
                {
                    text: 'DC kids',
                },
                {
                    text: 'DC universe',
                },
                {
                    text: 'DC POWER VISA',
                }
            ],
        }
    }
}
</script>

<template>
    <footer>
        <div class="container">
            <div class="row">
                <div class="col-4 ">
                    <div class="row my-2">
                        <div class="col-4">
                            <div class="subtitle py-3 fs-5 font-weight-bold">DC COMICS</div>
                            <ul>
                                <li class="d-flex align-items-center" v-for="comic in comics">
                                    <a class="px-6" href="#">{{ comic.text }}</a>
                                </li>
                            </ul>
                            <div class="subtitle py-3 fs-5 font-weight-bold">SHOP</div>
                            <ul>
                                <li class="d-flex align-items-center" v-for="store in shop">
                                    <a class="px-6" href="#">{{ store.text }}</a>
                                </li>
                            </ul>
                        </div>
                        <div class="col-4">
                            <div class="subtitle py-3 fs-5 font-weight-bold">DC</div>
                            <ul>
                                <li class="d-flex align-items-center" v-for="magazine in dc">
                                    <a class="px-6" href="#">{{ magazine.text }}</a>
                                </li>
                            </ul>                          
                        </div>
                        <div class="col-4">
                            <div class="subtitle py-3 fs-5 font-weight-bold">SITES</div>
                            <ul>
                                <li class="d-flex align-items-center" v-for="site in sites">
                                    <a class="px-6" href="#">{{ site.text }}</a>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
                <div class="col-8 ">
                    <img src="../assets/img/dc-logo-bg.png" alt="">
                </div>
            </div>
        </div>
    </footer>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;
    footer {
        background-image: url('src/assets/img/footer-bg.jpg');
    }
    .subtitle {
        color: #fff;
    }
    ul {
        padding: 0;
    }
    li {
        font-size: 10px;
        a {
            color: #959595;
        }
    }
    
</style>