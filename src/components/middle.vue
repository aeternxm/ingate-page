<template>
    <div class="mid-cont">
        <div class="mid-subcont">
            <div class="logomid-cont">
                <img src="../assets/logo.png" class="logomid"/>
            </div>
            <div class="txttitle-midcont">{{txtMTitle}}</div>
            <div class="txtsubtitle-midcont">{{txtMSubTitle}}</div>
            <div class="centralmid-subcont">
                <img src="../assets/dots.png" class="dots"/>
                <div class="rounded-cont">
                    <div class="internal-cont">
                        <div class="fstitem-cont">
                            <img src="../assets/check.png" class="check-item"/>
                            <div class="fst-item">{{txtFstItem}}</div>
                        </div>
                        <div class="snditem-cont">
                            <img src="../assets/check.png" class="check-item"/>
                            <div class="snd-item">{{txtSndItem}}</div>
                        </div>
                        <div class="trditem-cont">
                            <img src="../assets/check.png" class="check-item"/>
                            <div class="trd-item">{{txtTrdItem}}</div>
                        </div>
                        <div class="fthitem-cont">
                            <a href="https://app.ingate.com.br/signup" class="internal-btn">{{internalBtn}}</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "middle",
    props:{
        internalBtn: String,
        txtMTitle: String,
        txtMSubTitle: String,
        txtFstItem: String,
        txtSndItem: String,
        txtTrdItem: String
    }
}
</script>

<style scoped>
    @media(max-width:600px){
        .mid-cont{
            height: 122.5vh !important;
        }
        .logomid-cont{
            margin-top: 5vh !important;
            height: 10vh !important;
        }
        .logomid{
            width: 40% !important;
        }
        .txttitle-midcont{
            font-size: 5.25vh !important;
            
        }
        .txtsubtitle-midcont{
            margin-top: 5vh;
            font-size: 4vh !important;
        }
        .dots{
            display: none;
        }
        .rounded-cont{
            width: 97vw !important;
        }
        .fst-item{
            font-size: 2.5vh !important;
            text-align: left;
            margin: 0 3vh 0 3vh !important;
        }
        .snd-item{
            font-size: 2.5vh !important;
            text-align: left;
            margin: 0 3vh 0 3vh !important;
        }
        .trd-item{
            font-size: 2.5vh !important;
            text-align: left;
            margin: 0 3vh 0 3vh !important;
        }
        .internal-btn{
            height: 8vh !important;
            width: 50vw !important;
        }
        .check-item{
            width: 2.5vh !important;
            height: 2.5vh !important;
        }
    }

    .mid-cont{
        display: flex;
        flex-flow: row wrap;
        justify-content: center;
        width: 100vw;
        height: 122.5vh;
        background-color: black;
        font-family: "tiempoBolda";
    }

    .logomid-cont{
        display: flex;
        justify-content: center;
        align-items: flex-end;
        width: 100vw;
        height: 16.5vh;
    }

    .logomid{
        width: 11%;
        height: auto;
    }

    .mid-subcont{
        width: 100vw;
    }

    .txttitle-midcont{
        display: flex;
        align-items: flex-end;
        justify-content: center;
        width: 100vw;
        height: 18.5vh;
        font-size: 7.25vh;
        font-weight: 900;
    }

    .txtsubtitle-midcont{
        display: flex;
        align-items: flex-end;
        justify-content: center;
        width: 100vw;
        height: 10.5vh;
        font-size: 6vh;
        font-weight: 900;
    }

    .centralmid-subcont{
        position: relative;
        display: flex;
        align-items: flex-end;
        justify-content: flex-end;
        width: 100vw;
        height: 72vh;
    }

    .dots{
        position: absolute;
        top: 10vh;
        left: 9.5vw;
        width: 10vw;
        height: 18vh;
    }

    .rounded-cont{
        display: flex;
        justify-content: flex-end;
        width: 83.5vw;
        height: 60vh;
        background-color: #101218;
        border-top-left-radius: 12.5vh;
        border-bottom-left-radius: 12.5vh;
    }

    .internal-cont{
        display: flex;
        flex-flow: row wrap;
        align-content: flex-start;
        width: 94%;
        height: 100%;
    }
    
    .fstitem-cont{
        display: flex;
        align-items: center;
        width: 100%;
        height: 25%;
    }

    .snditem-cont{
        display: flex;
        align-items: center;
        width: 100%;
        height: 25%;
    }

    .trditem-cont{
        display: flex;
        align-items: center;
        width: 100%;
        height: 25%;
    }

    .fthitem-cont{
        display: flex;
        justify-content: center;
        align-items: center;
        width: 100%;
        height: 25%;
    }

    .internal-btn{
        display: flex;
        justify-content: center;
        align-items: center;
        height: 10vh;
        width: 18vw;
        border-radius: 1.5vh;
        background-color: white;
        text-decoration: none;
        text-transform: uppercase;
        font-size: 2.35vh;
        font-weight: 600;
        font-family: "roboto",sans-serif;
        color: black;
        transition: 0.5s;
    }

    .internal-btn:hover{
        background-color: #D32579;
        color: white;
    }

    .fst-item{
        margin-left: 1vw;
        font-family: "Roboto", sans-serif;
        font-size: 3.5vh;
        font-weight: bold;
    }

    .snd-item{
        margin-left: 1vw;
        font-family: "Roboto", sans-serif;
        font-size: 3.5vh;
        font-weight: bold;
    }

    .trd-item{
        margin-left: 1vw;
        font-family: "Roboto", sans-serif;
        font-size: 3.5vh;
        font-weight: bold;
    }

    .check-item{
        width: 3.5vh;
        height: 3.5vh;
    }
</style>