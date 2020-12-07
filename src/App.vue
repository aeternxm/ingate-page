<template>
  <div id="app">
    <top :login="top.loginPt" :txtBtn="top.txtBtnPt" :txtTitle="top.txtTitlePt" :txtSubtitle="top.txtSubtitlePt"/>
    <middle :internalBtn="middle.internalBtnPt" :txtMTitle="middle.txtMTitlePt" :txtMSubTitle="middle.txtMSubTitlePt" :txtFstItem="middle.txtFstItemPt" :txtSndItem="middle.txtSndItemPt" :txtTrdItem="middle.txtTrdItemPt"/>
    <bottom :txtBTitle="bottom.txtBTitlePt" :txtBTitleTwo="bottom.txtBTitleTwoPt" :btnB="bottom.btnBPt" :nameone="bottom.nameonePt" :nametwo="bottom.nametwoPt" :namethree="bottom.namethreePt" :namefour="bottom.namefourPt" :atone="bottom.atonePt" :attwo="bottom.attwoPt" :atthree="bottom.atthreePt" :atfour="bottom.atfourPt" :stdwrone="bottom.stdwronePt" :stdwrtwo="bottom.stdwrtwoPt" :stdwrthree="bottom.stdwrthreePt" :stdwrfour="bottom.stdwrfourPt"/>
    <footerr @trns-us="changeLang" @trns-pt="mudarLingua" :motto="footerr.mottoPt" :langUs="footerr.langUsPt" :langPt="footerr.langPtPt" :jobs="footerr.jobsPt" :terms="footerr.termsPt" :privacy="footerr.privacyPt" :copyLeft="footerr.copyLeftPt" :copyRight="footerr.copyRightPt"/>
  </div>
</template>

<script>
import top from "./components/top.vue"
import middle from "./components/middle.vue"
import bottom from "./components/bottom.vue"
import footerr from "./components/footerr.vue"

export default {
  name: "App",

  created(){
    document.title = "Ingate Educa"
  },

  methods:{
    changeLang(){
      this.top.txtTitlePt = "Enter the world of web development";
      this.top.txtSubtitlePt = "Weekly web development classes";
      this.top.txtBtnPt = "Watch now";
      this.middle.txtMTitlePt = "Don't know where to start?";
      this.middle.txtMSubTitlePt = "Get to know the";
      this.middle.txtFstItemPt = "Fullstack development:";
      this.middle.txtSndItemPt = "Project management:";
      this.middle.txtTrdItemPt = "Curriculum:";
      this.middle.internalBtnPt = "Know more";
      this.bottom.txtBTitlePt = "See what our students say about us";
      this.bottom.txtBTitleTwoPt = "Register now. It's free!";
      this.bottom.btnBPt = "Know more";
      this.footerr.jobsPt = "Jobs";
      this.footerr.termsPt = "Terms & Conditions";
      this.footerr.privacyPt = "Privacy Policy"
    },

    mudarLingua(){
      this.top.txtTitlePt = "O mundo do desenvolvimento web nunca esteve tão perto";
      this.top.txtSubtitlePt = "Conheça a escola do futuro que vai mudar o seu envolvimento com a programação";
      this.top.txtBtnPt = "Assista Agora";
      this.middle.txtMTitlePt = "Somos a escola ideal para você";
      this.middle.txtMSubTitlePt = "Conheça as suas vantagens de estudar com quem entende";
      this.middle.txtFstItemPt = "Aulas semanais, didática envolvente e uma comunidade forte.";
      this.middle.txtSndItemPt = "O apoio que você precisa pelo menor preço da internet.";
      this.middle.txtTrdItemPt = "Seja o programador do futuro, atue nos maiores projetos e faça diferença no mercado de TI.";
      this.middle.internalBtnPt = "Quero fazer parte!";
      this.bottom.txtBTitlePt = "Veja o que nossos alunos comentam";
      this.bottom.txtBTitleTwoPt = "Se cadastre agora. É de graça!";
      this.bottom.btnBPt = "Quero fazer parte!";
      this.footerr.jobsPt = "Trabalhe Conosco";
      this.footerr.termsPt = "Termos & Condições";
      this.footerr.privacyPt = "Políticas de Privacidade"
    }
  },

  data(){
    return{
      top:{
        loginPt:"login",
        txtBtnPt: "Assista Agora",
        txtTitlePt: "O mundo do desenvolvimento web nunca esteve tão perto",
        txtSubtitlePt: "Conheça a escola do futuro que vai mudar o seu envolvimento com a programação"
      },
      middle:{
        internalBtnPt:"Quero fazer parte!",
        txtMTitlePt: "Somos a escola ideal para você",
        txtMSubTitlePt: "Conheça as suas vantagens de estudar com quem entende",
        txtFstItemPt: "Aulas semanais, didática envolvente e uma comunidade forte.",
        txtSndItemPt: "O apoio que você precisa pelo menor preço da internet.",
        txtTrdItemPt: "Seja o programador do futuro, atue nos maiores projetos e faça diferença no mercado de TI.",
      },
      bottom:{
        txtBTitlePt: "Veja o que nossos alunos comentam",
        txtBTitleTwoPt: "Se cadastre agora. É de graça!",
        btnBPt: "Quero fazer parte!",
        nameonePt: "Nathalia",
        nametwoPt: "Vanessa Sinoki",
        namethreePt: "Wilcymar",
        namefourPt: "Lucas Andrade",
        atonePt: "@nathizr_",
        attwoPt: "@sinokivanessa_",
        atthreePt: "@wilcymar",
        atfourPt: "@luc_szan",
        stdwronePt: 'A didática do professor faz com que você se envolva, se interesse com o assunto e aplique-o na prática. "Não dê o peixe, ensine a pescar"',//I put single quote mark here because the string needs the double quote mark
        stdwrtwoPt: "Este curso me ensina a ser uma progamadora por completo e não apenas a programar. Estou muito feliz com o desenvolvimento que a Ingate me proporcionou.",
        stdwrthreePt: "Só tenho a comemorar o fato de ter conhecido o YoYo. Seu método replica a realidade da prog. e dev. no mundo real. Aprendi principalmente o que não fazer e como fazer para ser visto como programador.",
        stdwrfourPt: "Foi com confiança que resolvi investir no Yoyo para guiar meu aprendizado. Muito disso se deve a uma mentalidade de crescimento, de que nada é inato e que podemos conquistar muito mais do que pensamos com nosso esforço. Assim, o que me atraiu foi a superação de um curso teórico ou tradicional, afinal aprender sempre depende de nós.",
      },
      footerr:{
        mottoPt: "The gate to your universe",
        langUsPt: "🇺🇸 US/Global - English",
        langPtPt: "🇧🇷 Brasil - Português",
        jobsPt: "Trabalhe conosco",
        termsPt: "Termos e condições",
        privacyPt: "Políticas de Privacidade",
        copyLeftPt: "Copyright 2020 Ingate. All Rights Reserved.",
        copyRightPt: "Created with ❤️ at 🇯🇵 & 🇧🇷"
      }
    }
  },
  components:{
    top,
    middle,
    bottom,
    footerr,
  },
}
</script>

<style>
*{
  margin: 0;
  box-sizing: border-box;
}

#app {
  width: 100vw;
  color: #ffffff;
  background-color: #000000;
  text-align: center;
  font-family: Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

</style>