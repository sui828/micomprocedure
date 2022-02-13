<template>
  <div class="container">
      <header>
        <div class="header-box">
          <router-link to="/">
            <div class="title-box">
              <img class="proc-icon" src="../assets/common/proc_ico.svg" width="40">
              <h1 class="maintitle">Micomprocedure</h1>
              <h1 class="subtitle">東北大学ゲーム制作サークル<br>マイコンプロシージャ</h1>
            </div>
          </router-link>
          <nav class="navi">
            <ul class="menu-box">
              <li class="menu-item" @click="scrollFreshman"><input type="button" id="scroll-1" value="FRESHMAN"></li>
              <li class="menu-item" @click="scrollSenior"><input type="button" id="scroll-2" value="SENIOR"></li>
            </ul>
            <ul class="menu-box2">
              <li class="menu-item2" @click="scrollFreshman"><input type="button" id="scroll-1" value="新入生プロジェクト"></li>
              <li class="menu-item2" @click="scrollSenior"><input type="button" id="scroll-2" value="その他"></li>
            </ul>
          </nav>
        </div>
      </header>
  <div class="works">
    <div class="caption1">WORKS</div>
    <div class="caption2">作品一覧</div>
    <div class="semi-space"></div>
    <div class="info-caption">2021年度新入生プロジェクト</div>
    <div class="works-box">
      <div class="works-content">
        <img src="../assets/works/THE_UFO_ico.png">
        <a href="#" class="disabled">
          <div class="works-mask">
            <div class="works-caption">THE Unexpected Fighting Operation</div>
          </div>
        </a>
      </div>
      <div class="works-content">
        <img src="../assets/works/harusagashi_ico.png">
        <a href="#" class="disabled">
          <div class="works-mask">
            <div class="works-caption">はるさがし</div>
          </div>
        </a>
      </div>
      <div class="works-content">
        <img src="../assets/works/Escape_from_Shrine_ico.png">
        <a href="#" class="disabled">
          <div class="works-mask">
            <div class="works-caption">神社からの脱出</div>
          </div>
        </a>
      </div>
      <div class="works-content">
        <img src="../assets/works/Gravity-Lost_ico.png">
        <a href="#" v="disabled">
          <div class="works-mask">
            <div class="works-caption">Gravity-Lost</div>
          </div>
        </a>
      </div>
      <div class="works-content">
        <img src="../assets/works/R_T_A_ico.png">
        <a href="#" class="disabled">
          <div class="works-mask">
            <div class="works-caption">落単・タイム・アタック！</div>
          </div>
        </a>
      </div>
    </div>
    <div class="semi-space"></div>
    <div class="info-caption">2020年度新入生プロジェクト</div>
    <div class="works-box">
      <div class="works-content">
        <img src="../assets/works/THE_UFO_ico.png">
        <a href="#" class="disabled">
          <div class="works-mask">
            <div class="works-caption">Crossfade</div>
          </div>
        </a>
      </div>
      <div class="works-content">
        <img src="../assets/works/harusagashi_ico.png">
        <a href="#" class="disabled">
          <div class="works-mask">
            <div class="works-caption">トキノカダイ</div>
          </div>
        </a>
      </div>
      <div class="works-content">
        <img src="../assets/works/Escape_from_Shrine_ico.png">
        <a href="#" class="disabled">
          <div class="works-mask">
            <div class="works-caption">Team C no game</div>
          </div>
        </a>
      </div>
      <div class="works-content">
        <img src="../assets/works/Gravity-Lost_ico.png">
        <a href="#" v="disabled">
          <div class="works-mask">
            <div class="works-caption">城熊 ~shirokuma~</div>
          </div>
        </a>
      </div>
    </div>
    <div id="point-2" class="space"></div>
    <div class="space"></div>
  </div>
  <footer>
    <div class="snsicon">
      <ul class="snsiconlist">
        <li><div class="footertext"><b>SHARE</b></div></li>
      </ul>
      <ul class="snsiconlist">
        <li><a href="https://twitter.com/share?url=https://sui828.github.io/proce/&text=Micomprocedure%28%E3%83%9E%E3%82%A4%E3%82%B3%E3%83%B3%E3%83%97%E3%83%AD%E3%82%B7%E3%83%BC%E3%82%B8%E3%83%A3%29+-+%E6%9D%B1%E5%8C%97%E5%A4%A7%E5%AD%A6%E3%82%B2%E3%83%BC%E3%83%A0%E5%88%B6%E4%BD%9C%E3%82%B5%E3%83%BC%E3%82%AF%E3%83%AB%0D%0A&related=micom_procedure"><img src="../assets/common/iconmonstr-twitter-4.svg"></a></li>
        <li><a href="https://www.facebook.com/sharer/sharer.php?u=https://sui828.github.io/proce/"><img src="../assets/common/iconmonstr-facebook-4.svg"></a></li>
        <li><a href="http://line.me/R/msg/text/?Micomprocedure%28%E3%83%9E%E3%82%A4%E3%82%B3%E3%83%B3%E3%83%97%E3%83%AD%E3%82%B7%E3%83%BC%E3%82%B8%E3%83%A3%29+-+%E6%9D%B1%E5%8C%97%E5%A4%A7%E5%AD%A6%E3%82%B2%E3%83%BC%E3%83%A0%E5%88%B6%E4%BD%9C%E3%82%B5%E3%83%BC%E3%82%AF%E3%83%AB%0D%0Ahttps%3A%2F%2Fsui828.github.io%2Fproce%2F"><img src="../assets/common/iconmonstr-line-4.svg"></a></li>
      </ul>
    </div>
    <div class="copyright">&copy; Copyright micomprocedure 2021 all right reserved.</div>
  </footer>

  </div>
</template>

<script>
export default {
  methods: {
    scrollFreshman: function(){
      window.scrollTo({
        top: 300,
        behavior: "smooth"
      });
    },
    scrollSenior: function(){
      window.scrollTo({
        top: 2600,
        behavior: "smooth"
      });
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
  @import "../assets/stylesheet.css"
</style>