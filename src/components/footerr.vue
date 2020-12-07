<template>
    <div class="footer-cont">
        <div class="footertop-cont">
            <img src="../assets/logo.png" class="footer-logo"/>
        </div>
        <div class="footersubtop-cont">{{motto}}</div>
        <div class="socmed-cont">
            <a href="https://instagram.com/ticomyoyo">
                <img src="../assets/insta.svg" class="socmed-img"/>
            </a>
            <a href="https://www.instagram.com/ticomyoyo">
            <img src="../assets/discord.svg" class="socmed-img"/>
            </a>
            <a href="https://www.youtube.com/yoyonobouken">
            <img src="../assets/youtube.svg" class="socmed-img"/>
            </a>
            <a href="https://t.me/ticomyoyo">
            <img src="../assets/telegram.svg" class="socmed-img"/>
            </a>
        </div>
        <div class="lang-cont">
            <div class="lang-us" v-on:click="transUs()">{{langUs}}</div>
            <div class="lang-pt" @click="transPt()">{{langPt}}</div>
        </div>
        <div class="links-cont">
            <a href="https://ingate.com.br/jobs" class="links">{{jobs}}</a>
            <a href="https://ingate.com.br/terms" class="links">{{terms}}</a>
            <a href="https://ingate.com.br/policy" class="links">{{privacy}}</a>
        </div>
        <div class="copyright-cont">
            <div class="copyright-left">{{copyLeft}}</div>
            <div class="copyright-right">{{copyRight}}</div>
        </div>
    </div>
</template>

<script>
export default {
    props:{
        motto: String,
        langUs: String,
        langPt: String,
        jobs: String,
        terms: String,
        privacy: String,
        copyLeft: String,
        copyRight: String
    },

    methods:{
        transUs(){
            console.log('enviado'),
            this.$emit('trns-us')
        },
        transPt(){
            this.$emit('trns-pt')
        }
    }, 
}
</script>

<style scoped>
    @media(max-width:600px){
        .footertop-cont{
            justify-content: center !important;
        }
        .footersubtop-cont{
            justify-content: center !important;
        }
        .lang-cont{
            width: 97vw !important;
        }
        .lang-us{
            width: 100vw !important;
        }
        .lang-pt{
            width: 100vw !important;
        }
        .socmed-cont{
            justify-content: center !important;
        }
    }

    .footer-cont{
        width: 100vw;
        height: 55vh;
        background-color: #111319;
        border-top: 0.35vh solid white
    }

    .footertop-cont{
        display: flex;
        align-items: flex-end;
        width: 100vw;
        height: 12.5vh;
    }

    .footer-logo{
        width: auto;
        height: 5.35vh;
        margin-left: 3vw;
    }

    .footersubtop-cont{
        display: flex;
        justify-content: flex-start;
        margin: 0.5vw 0 0 3vw;
        width: 97vw;
        height: 2.25vh;
        font-size: 2vh;
    }

    .socmed-cont{
        display: flex;
        justify-content: flex-start;
        align-items: center;
        margin: 5vh 0 2.5vh 3vw;
        width: 97vw;
        height: 10vh;
    }

    .socmed-img{
        filter: invert(1);
        width: 6vh;
        height: 6vh;
        padding: 1vh;
        margin-right: 2vw;
        border: 0.35vh solid black;
        border-radius: 50%;
    }

    .lang-cont{
        display: flex;
        flex-flow: row wrap;
        width: 15vw;
        margin: 0vh 0 5vh 3vw;
        height: 5vh;
    }

    .lang-us{
        display: flex;
        justify-content: flex-start;
        font-size: 2vh;
        cursor: pointer;
    }

    .lang-pt{
        display: flex;
        justify-content: flex-start;
        font-size: 2vh;
        cursor: pointer;
    }

    .links-cont{
        display: flex;
        justify-content: flex-end;
        height: 5vh;
        width: 100vw;
    }

    .links{
        color: white;
        text-decoration: none;
        font-size: 1.8vh;
        margin-right: 3vw;
    }

    .copyright-cont{
        display: flex;
        flex-flow: row nowrap;
        width: 100vw;
        height: 6.15vh;
        color: #8094AD;
        font-size: 1.75vh;
    }

    .copyright-left{
        display: flex;
        align-items: center;
        width: 50vw;
        margin-left: 3vw;
    }

    .copyright-right{
        display: flex;
        align-items: center;
        justify-content: flex-end;
        width: 50vw;
        margin-right: 3vw;
    }
</style>