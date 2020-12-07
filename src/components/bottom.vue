<template>
    <div class="bottom-cont">
        <div class="bottom-title">{{txtBTitle}}</div>
        <div class="stud-cont">
            <div class="stud-subcont">
                <div class="stud-txt">{{stdwrone}}</div>
                <div class="studbot-cont">
                    <img src="../assets/nath.jpg" class="stud-img"/>
                    <div class="studname-cont">
                        <div class="stud-name">{{nameone}}</div>
                        <div class="stud-at">{{atone}}</div>
                    </div>
                </div>
            </div>
            <div class="stud-subcont">
                <div class="stud-txt">{{stdwrtwo}}</div>
                <div class="studbot-cont">
                    <img src="../assets/usertwo.png" class="stud-img"/>
                    <div class="studname-cont">
                        <div class="stud-name">{{nametwo}}</div>
                        <div class="stud-at">{{attwo}}</div>
                    </div>
                </div>
            </div>
            <div class="stud-subcont">
                <div class="stud-txt">{{stdwrthree}}</div>
                <div class="studbot-cont">
                    <img src="../assets/wilcy.jpg" class="stud-img"/>
                    <div class="studname-cont">
                        <div class="stud-name">{{namethree}}</div>
                        <div class="stud-at">{{atthree}}</div>
                    </div>
                </div>
            </div>
            <div class="stud-subcont">
                <div class="stud-txt">{{stdwrfour}}</div>
                <div class="studbot-cont">
                    <img src="../assets/lucas.jpg" class="stud-img"/>
                    <div class="studname-cont">
                        <div class="stud-name">{{namefour}}</div>
                        <div class="stud-at">{{atfour}}</div>
                    </div>
                </div>
            </div>
        </div>
        <div class="lstbotitem-cont">
            <div class="lstbotitem-title">{{txtBTitleTwo}}</div>
            <a href="https://app.ingate.com.br/signup" class="lstbotitem-btn">{{btnB}}</a>
        </div>
    </div>
</template>

<script>
export default {
    name: "bottom",
    props:{
        txtBTitle: String,
        txtBTitleTwo: String,
        btnB: String,
        nameone: String,
        nametwo: String,
        namethree: String,
        namefour: String,
        atone: String,
        attwo: String,
        atthree: String,
        atfour: String,
        stdwrone: String,
        stdwrtwo: String,
        stdwrthree: String,
        stdwrfour: String,
    },
}
</script>

<style scoped>
    @media(max-width:600px){
        .stud-cont{
            display: flex;
            justify-content: center;
            flex-flow: row wrap;
            width: 100vw;
            margin-top: 3vh;
        }

        .stud-subcont{
            width: 70vw !important;
        }

        .stud-txt{
            width: 50vw !important;
        }

        .lstbotitem-btn{
            width: 94vw !important;
        }
    }

    .bottom-cont{
        width: 100vw;
    }

    .bottom-title{
        width: 100vw;
        margin-top: 5vh;
        font-size: 6.75vh;
        font-weight: 600;
        font-family: "tiempoBolda";
    }

    .stud-cont{
        display: flex;
        justify-content: center;
        flex-flow: row wrap;
        width: 100vw;
        margin-top: 3vh;
    }

    .stud-subcont{
        display: flex;
        justify-content: center;
        flex-flow: row wrap;
        width: 22.5vw;
        height: 60vh;
        background-color: #202225;
        margin: 3vh 0.75vw 3vh 0.75vw;
        border-radius: 3vh;
        transition: 0.5s;
    }

    .stud-subcont:hover{
        background-color: #6838F8;
    }

    .studbot-cont{
        display: flex;
        align-items: center;
        justify-content: center;
        flex-flow: row nowrap;
        width: 100%;
        height: 18vh;
    }

    .stud-img{
        width: 10.5vh;
        height: 10.5vh;
        border-radius: 100%;
        margin-right: 1.5vw;
        margin-left: 1.5vw;
    }

    .studname-cont{
        display: flex;
        flex-flow: wrap;
        justify-self: left;
        width: 50%;
    }

    .stud-name{
        display: flex;
        justify-self: left;
        width: 80%;
        font-size: 2.25vh;
        font-weight: 600;
    }

    .stud-at{
        display: flex;
        justify-self: left;
        width: 100%;
        font-size: 1.85vh;
    }

    .stud-txt{
        display: flex;
        overflow: auto;
        width: 19.25vw;
        height: 38vh;
        margin-top: 5vh;
        font-family: "tiempoBolda";
        font-size: 3vh;
        font-weight: 600;
        text-align: left;
        cursor: pointer;
    }

    ::-webkit-scrollbar {
        width: 1.5vh;
        cursor: pointer;
    }

    ::-webkit-scrollbar-track {
        background-color: #333336; 
        border-radius: 10px;
    }

    ::-webkit-scrollbar-thumb {
        background: #55545B; 
        border-radius: 10px;
    }

    ::-webkit-scrollbar-track:hover {
        background: #5E41B5;
    }

    ::-webkit-scrollbar-thumb:hover {
        background: #4B0881;
    }

    .lstbotitem-cont{
        display: flex;
        justify-content: center;
        align-items: center;
        flex-flow: row wrap;
        height: 50vh;
        width: 100vw;
    }

    .lstbotitem-title{
        width: 100vw;
        margin-top: 6vh;
        font-size: 6.75vh;
        font-weight: 600;
        font-family: "tiempoBolda";
    }

    .lstbotitem-btn{
        display: flex;
        justify-content: center;
        align-items: center;
        margin-bottom: 8vh;
        height: 10vh;
        width: 22vw;
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

    .lstbotitem-btn:hover{
        background-color: #D32579;
        color: white;
    }
</style>