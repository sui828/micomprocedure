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
        <div @click="open1">
          <div class="works-mask">
            <div class="works-caption">THE Unexpected Fighting Operation</div>
          </div>
        </div>
        <v-dialog
          width="80%"
          max-width="1366"
          scrollable
          v-model="dialog1"
        >
          <div class="dialog">
            <div class="dialog-box">
              <img src="../assets/works/THE_UFO_ico.png">
              <div class="dialog-text">
                <h1>THE Unexpected Fighting Operation</h1>
                <h2>2Dアクション</h2>
                <p>異世界のような宇宙のどこかの惑星で、宇宙船が故障したらしい乗組員が現地の生命と戦い、素材を手に入れ、宇宙船の修理そして帰還を目指すスペース・ファンタジーゲームです。</p>
              </div>
            </div>
            <div class="mainbuttonarea2">
              <a href="http://www.proc.org.tohoku.ac.jp/?plugin=attach&refer=%B8%F8%B3%AB%C3%E6%A4%CE%BA%EE%C9%CA%2F2021%C7%AF%C5%D9%BF%B7%C6%FE%C0%B8%A5%D7%A5%ED%A5%B8%A5%A7%A5%AF%A5%C8%2FTHE%20Unexpected%20Fighting%20Operation&openfile=THE%20Unexpected%20Fighting%20Operation.zip"><span class="mainbuttonspan"><b>DOWNLOAD</b></span></a>
            </div>
          </div>
        </v-dialog>
      </div>
      <div class="works-content">
        <img src="../assets/works/harusagashi_ico.png">
        <div @click="open2">
          <div class="works-mask">
            <div class="works-caption">はるさがし</div>
          </div>
        </div>
        <v-dialog
          width="80%"
          max-width="1366"
          scrollable
          v-model="dialog2"
        >
          <div class="dialog">
            <div class="dialog-box">
              <img src="../assets/works/harusagashi_ico.png">
              <div class="dialog-text">
                <h1>はるさがし</h1>
                <h2>2Dアクション</h2>
                <p>歩行と飛行を切り替えながらキャラクターを操作し、さがしものを集めて春を取り戻せ！</p>
              </div>
            </div>
            <div class="mainbuttonarea2">
              <a href="http://www.proc.org.tohoku.ac.jp/?plugin=attach&refer=%B8%F8%B3%AB%C3%E6%A4%CE%BA%EE%C9%CA%2F2021%C7%AF%C5%D9%BF%B7%C6%FE%C0%B8%A5%D7%A5%ED%A5%B8%A5%A7%A5%AF%A5%C8%2F%A4%CF%A4%EB%A4%B5%A4%AC%A4%B7&openfile=Harusagashi_V1.0.zip"><span class="mainbuttonspan"><b>DOWNLOAD</b></span></a>
            </div>
          </div>
        </v-dialog>
      </div>
      <div class="works-content">
        <img src="../assets/works/Escape_from_Shrine_ico.png">
        <div @click="open3">
          <div class="works-mask">
            <div class="works-caption">神社からの脱出</div>
          </div>
        </div>
        <v-dialog
          width="80%"
          max-width="1366"
          scrollable
          v-model="dialog3"
        >
          <div class="dialog">
            <div class="dialog-box">
              <img src="../assets/works/Escape_from_Shrine_ico.png">
              <div class="dialog-text">
                <h1>神社からの脱出</h1>
                <h2>3Dホラー</h2>
                <p>ミニゲームをクリアしながら、神社からの脱出を目指すゲーム。</p>
              </div>
            </div>
            <div class="mainbuttonarea2">
              <a href="http://www.proc.org.tohoku.ac.jp/?plugin=attach&refer=%B8%F8%B3%AB%C3%E6%A4%CE%BA%EE%C9%CA%2F2021%C7%AF%C5%D9%BF%B7%C6%FE%C0%B8%A5%D7%A5%ED%A5%B8%A5%A7%A5%AF%A5%C8%2F%BF%C0%BC%D2%A4%AB%A4%E9%A4%CE%C3%A6%BD%D0&openfile=%BF%C0%BC%D2%A4%AB%A4%E9%A4%CE%C3%A6%BD%D0.zip"><span class="mainbuttonspan"><b>DOWNLOAD</b></span></a>
            </div>
          </div>
        </v-dialog>
      </div>
      <div class="works-content">
        <img src="../assets/works/Gravity-Lost_ico.png">
        <div @click="open4">
          <div class="works-mask">
            <div class="works-caption">Gravity-Lost</div>
          </div>
        </div>
        <v-dialog
          width="80%"
          max-width="1366"
          scrollable
          v-model="dialog4"
        >
          <div class="dialog">
            <div class="dialog-box">
              <img src="../assets/works/Gravity-Lost_ico.png">
              <div class="dialog-text">
                <h1>Gravity-Lost</h1>
                <h2>3Dアクション</h2>
                <p>ロボットのラヴィはとある事故をきっかけにほぼ全ての記憶をなくしてしまった。ラヴィは自身の記憶チップを回収しながら唯一覚えている白衣の男性を探す旅に出る・・・。</p>
              </div>
            </div>
            <div class="mainbuttonarea2">
              <a href="http://www.proc.org.tohoku.ac.jp/?plugin=attach&refer=%B8%F8%B3%AB%C3%E6%A4%CE%BA%EE%C9%CA%2F2021%C7%AF%C5%D9%BF%B7%C6%FE%C0%B8%A5%D7%A5%ED%A5%B8%A5%A7%A5%AF%A5%C8%2FGravity-Lost&openfile=Gravity-Lost.zip"><span class="mainbuttonspan"><b>DOWNLOAD</b></span></a>
            </div>
          </div>
        </v-dialog>
      </div>
      <div class="works-content">
        <img src="../assets/works/R_T_A_ico.png">
        <div @click="open5">
          <div class="works-mask">
            <div class="works-caption">落単・タイム・アタック！</div>
          </div>
        </div>
        <v-dialog
          width="80%"
          max-width="1366"
          scrollable
          v-model="dialog5"
        >
          <div class="dialog">
            <div class="dialog-box">
              <img src="../assets/works/R_T_A_ico.png">
              <div class="dialog-text">
                <h1>落単・タイム・アタック！</h1>
                <h2>2Dアクション</h2>
                <p>―――限界大学生に刻一刻と迫る再履の音―――<br>あなたは落単間近の大学生（以下、イカトン）。レポートの提出を目指しキャンパスを駆け巡ります。道中の「金のレポート」を回収し、高評定を目指しましょう。</p>
              </div>
            </div>
            <div class="mainbuttonarea2">
              <a href="http://www.proc.org.tohoku.ac.jp/?plugin=attach&refer=%B8%F8%B3%AB%C3%E6%A4%CE%BA%EE%C9%CA%2F2021%C7%AF%C5%D9%BF%B7%C6%FE%C0%B8%A5%D7%A5%ED%A5%B8%A5%A7%A5%AF%A5%C8%2F%CD%EE%C3%B1%A1%A6%A5%BF%A5%A4%A5%E0%A1%A6%A5%A2%A5%BF%A5%C3%A5%AF%A1%AA&openfile=%CD%EE%C3%B1RTA.zip"><span class="mainbuttonspan"><b>DOWNLOAD</b></span></a>
            </div>
          </div>
        </v-dialog>
      </div>
    </div>
    <div class="semi-space"></div>
    <div class="info-caption">2020年度新入生プロジェクト</div>
    <div class="works-box">
      <div class="works-content">
        <img src="../assets/works/crossfade_ico.png">
        <div @click="open11">
          <div class="works-mask">
            <div class="works-caption">CrossFade</div>
          </div>
        </div>
        <v-dialog
          width="80%"
          max-width="1366"
          scrollable
          v-model="dialog11"
        >
          <div class="dialog">
            <div class="dialog-box">
              <img src="../assets/works/crossfade_ico.png">
              <div class="dialog-text">
                <h1>CrossFade</h1>
                <h2>2D音楽</h2>
                <p>音楽に合わせて、四方向から迫りくる敵を倒そう。</p>
              </div>
            </div>
            <div class="mainbuttonarea2">
              <a href="http://www.proc.org.tohoku.ac.jp/?plugin=attach&refer=%B8%F8%B3%AB%C3%E6%A4%CE%BA%EE%C9%CA%2F2020%C7%AF%C5%D9%BF%B7%C6%FE%C0%B8%A5%D7%A5%ED%A5%B8%A5%A7%A5%AF%A5%C8%2FCrossFade&openfile=CrossFade.zip"><span class="mainbuttonspan"><b>DOWNLOAD</b></span></a>
            </div>
          </div>
        </v-dialog>
      </div>
      <div class="works-content">
        <img src="../assets/works/tokinokadai_ico.png">
        <div @click="open12">
          <div class="works-mask">
            <div class="works-caption">トキノカダイ</div>
          </div>
        </div>
        <v-dialog
          width="80%"
          max-width="1366"
          scrollable
          v-model="dialog12"
        >
          <div class="dialog">
            <div class="dialog-box">
              <img src="../assets/works/tokinokadai_ico.png">
              <div class="dialog-text">
                <h1>トキノカダイ</h1>
                <h2>2Dアクション</h2>
                <p>時を止める力を持つ少女は宿題が終わらない。タイミングよく時を止めて敵を倒し、ボスステージを攻略しよう。</p>
              </div>
            </div>
            <div class="mainbuttonarea2">
              <a href="http://www.proc.org.tohoku.ac.jp/?plugin=attach&refer=%B8%F8%B3%AB%C3%E6%A4%CE%BA%EE%C9%CA%2F2020%C7%AF%C5%D9%BF%B7%C6%FE%C0%B8%A5%D7%A5%ED%A5%B8%A5%A7%A5%AF%A5%C8%2F%A5%C8%A5%AD%A5%CE%A5%AB%A5%C0%A5%A4&openfile=TokinokadaiVer1.2.zip"><span class="mainbuttonspan"><b>DOWNLOAD</b></span></a>
            </div>
          </div>
        </v-dialog>
      </div>
      <div class="works-content">
        <img src="../assets/works/tCg_ico.png">
        <div @click="open13">
          <div class="works-mask">
            <div class="works-caption">TeamC no game</div>
          </div>
        </div>
        <v-dialog
          width="80%"
          max-width="1366"
          scrollable
          v-model="dialog13"
        >
          <div class="dialog">
            <div class="dialog-box">
              <img src="../assets/works/tCg_ico.png">
              <div class="dialog-text">
                <h1>TeamC no game</h1>
                <h2>2Dパズル</h2>
                <p>様々な能力をもつロボットと一緒に地形を略しよう。</p>
              </div>
            </div>
            <div class="mainbuttonarea2">
              <a href="http://www.proc.org.tohoku.ac.jp/?plugin=attach&refer=%B8%F8%B3%AB%C3%E6%A4%CE%BA%EE%C9%CA%2F2020%C7%AF%C5%D9%BF%B7%C6%FE%C0%B8%A5%D7%A5%ED%A5%B8%A5%A7%A5%AF%A5%C8%2FTeamC%20no%20game&openfile=TeamCNoGame.zip"><span class="mainbuttonspan"><b>DOWNLOAD</b></span></a>
            </div>
          </div>
        </v-dialog>
      </div>
      <div class="works-content">
        <img src="../assets/works/shirokuma_ico.png">
        <div @click="open14">
          <div class="works-mask">
            <div class="works-caption">城熊~shirokuma~</div>
          </div>
        </div>
        <v-dialog
          width="80%"
          max-width="1366"
          scrollable
          v-model="dialog14"
        >
          <div class="dialog">
            <div class="dialog-box">
              <img src="../assets/works/shirokuma_ico.png">
              <div class="dialog-text">
                <h1>城熊~shirokuma~</h1>
                <h2>3Dアクション</h2>
                <p>城に囚われた熊を脱出させよう！</p>
              </div>
            </div>
            <div class="mainbuttonarea2">
              <a href="http://www.proc.org.tohoku.ac.jp/?plugin=attach&refer=%B8%F8%B3%AB%C3%E6%A4%CE%BA%EE%C9%CA%2F2020%C7%AF%C5%D9%BF%B7%C6%FE%C0%B8%A5%D7%A5%ED%A5%B8%A5%A7%A5%AF%A5%C8%2F%BE%EB%B7%A7&openfile=shirokuma_1.11.zip"><span class="mainbuttonspan"><b>DOWNLOAD</b></span></a>
            </div>
          </div>
        </v-dialog>
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
  data() {
    return {
      dialog1: false,
      dialog2: false,
      dialog3: false,
      dialog4: false,
      dialog5: false,
      dialog11: false,
      dialog12: false,
      dialog13: false,
      dialog14: false
    };
  },
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
    },
    open1: function(){
      this.dialog1 = true;
    },
    open2: function(){
      this.dialog2 = true;
    },
    open3: function(){
      this.dialog3 = true;
    },
    open4: function(){
      this.dialog4 = true;
    },
    open5: function(){
      this.dialog5 = true;
    },
    open11: function(){
      this.dialog11 = true;
    },
    open12: function(){
      this.dialog12 = true;
    },
    open13: function(){
      this.dialog13 = true;
    },
    open14: function(){
      this.dialog14 = true;
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
  @import "../assets/stylesheet.css"
</style>