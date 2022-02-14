<template>
  <div class="container">
    <div class="main">
      <header>
        <div class="header-box">
          <div class="title-box" @click="scrollTop">
            <img class="proc-icon" src="../assets/common/proc_ico.svg" width="40">
            <h1 class="maintitle">Micomprocedure</h1>
            <h1 class="subtitle">東北大学ゲーム制作サークル<br>マイコンプロシージャ</h1>
          </div>
          <nav class="navi">
            <ul class="menu-box">
              <li class="menu-item" @click="scrollAbout"><input type="button" id="scroll-1" value="ABOUT"></li>
              <li class="menu-item" @click="scrollWorks"><input type="button" id="scroll-2" value="WORKS"></li>
              <li class="menu-item" @click="scrollJoin"><input type="button" id="scroll-5" value="JOIN US"></li>
            </ul>
            <ul class="menu-box2">
              <li class="menu-item2" @click="scrollAbout"><input type="button" id="scroll-1" value="サークル情報"></li>
              <li class="menu-item2" @click="scrollWorks"><input type="button" id="scroll-2" value="作品一覧"></li>
              <li class="menu-item2" @click="scrollJoin"><input type="button" id="scroll-5" value="新歓情報"></li>
            </ul>
          </nav>
        </div>
      </header>
  
  <div class="car_space"></div>
  <Carousel/>
  <div class="about">
    <div class="caption1">ABOUT</div>
    <div class="caption2">サークル情報</div>
    <ul class="about-box">
      <li class="about-left">名称</li>
      <li class="about-right">東北大学文化部登録団体<br>東北大学マイコンプロシージャ</li>
    </ul>
    <ul class="about-box">
      <li class="about-left">部室</li>
      <li class="about-right">川内北キャンパス内 川内サークル部室棟4階 416号室</li>
    </ul>
    <ul class="about-box">
      <li class="about-left">設立</li>
      <li class="about-right">1979年4月1日</li>
    </ul>
    <ul class="about-box">
      <li class="about-left">活動時間</li>
      <li class="about-right">不定期</li>
    </ul>
    <ul class="about-box">
      <li class="about-left">活動内容</li>
      <li class="about-right">ゲームの制作・発表など</li>
    </ul>
    <ul class="about-box">
      <li class="about-left">部費</li>
      <li class="about-right">3000円</li>
    </ul>
    <div id="point-2" class="space"></div>
  </div>
  <div class="works">
    <div class="caption1">WORKS</div>
    <div class="caption2">作品一覧</div>
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
    <div class="mainbuttonarea">
      <router-link to="/works"><span class="mainbuttonspan" @click="scrollTop2"><b>and more...</b></span></router-link>
    </div>
    <div id="point-3" class="end-space"></div>
  </div>
  <div class="info">
    <div class="caption1">JOIN US</div>
    <div class="caption2">新歓情報</div>
    <div class="space"></div>
    <div class="info-caption">
      新入部員募集中！
    </div>
    <div class="info-text">
      マイコンプロシージャは新入部員を随時募集しています！<br>未経験者、2年生以上の入部も大歓迎です。<br>実際、多くの新入生がプロセに入ってから創作活動を始めています。<br>一緒に創作活動をしてみませんか？<br>お待ちしています！
    </div>
    <div class="space"></div>
    <div class="info-caption">年間スケジュール予定</div>
    <ul class="join-box">
      <li class="join-left" style="background: #ff8080;">4月</li>
      <li class="join-right">新歓活動<br>スプリングフェスティバル</li>
    </ul>
    <ul class="join-box">
      <li class="join-left" style="background: #ffd280;">5月</li>
      <li class="join-right">新入生講習会</li>
    </ul>
    <ul class="join-box">
      <li class="join-left" style="background: #ffff80;">6月</li>
      <li class="join-right">新入生役職希望調査<br>新入生プロジェクトチーム分け</li>
    </ul>
    <ul class="join-box">
      <li class="join-left" style="background: #80d280;">7月</li>
      <li class="join-right">オープンキャンパス</li>
    </ul>
    <ul class="join-box">
      <li class="join-left" style="background: #80d2ff;">8月</li>
      <li class="join-right">α版発表会</li>
    </ul>
    <ul class="join-box">
      <li class="join-left" style="background: #8080ff;">10月</li>
      <li class="join-right">β版発表会</li>
    </ul>
    <ul class="join-box">
      <li class="join-left" style="background: #d280d2;">11月</li>
      <li class="join-right">東北大学祭</li>
    </ul>
    <ul class="join-box">
      <li class="join-left" style="background: #aaa;">不定期</li>
      <li class="join-right">プロセゲームジャム<br>DTM交流会<br>3D交流会</li>
    </ul>
    <div class="space"></div>
    <div class="info-caption">入部までの流れ</div>
    <div class="flowtitle"><span class="flowline"> <img src="../assets/common/iconmonstr-arrow-36.svg" class="rarr"> 見学 </span></div>
    <div class="info-text">Twitter(@micom_procedure)のDM/メール()から、見学希望の旨と希望する時間を書いてお伝えください。</div>
    <div class="info-text"><img src="../assets/common/iconmonstr-arrow-65.svg" class="darr"></div>
    <div class="flowtitle"><span class="flowline"> <img src="../assets/common/iconmonstr-arrow-36.svg" class="rarr"> 入部フォームに記入 </span></div>
    <div class="info-text">入部フォームをDMまたはメールで共有しますので、記入・回答をお願いします。</div>
    <div class="info-text"><img src="../assets/common/iconmonstr-arrow-65.svg" class="darr"></div>
    <div class="flowtitle"><span class="flowline"> <img src="../assets/common/iconmonstr-arrow-36.svg" class="rarr"> Slack/Discordに参加 </span></div>
    <div class="info-text">後日、Slackの招待がされますので、参加して部員名簿に氏名等を書くと入部完了です！</div>
    <div class="space"></div>
  </div>
  <footer>
    <div class="snsicon">
      <ul class="snsiconlist">
        <li><div class="footertext"><b>SHARE</b></div></li>
      </ul>
      <ul class="snsiconlist">
        <li><a href="https://twitter.com/share?url=https://sui828.github.io/micomprocedure/&text=Micomprocedure%28%E3%83%9E%E3%82%A4%E3%82%B3%E3%83%B3%E3%83%97%E3%83%AD%E3%82%B7%E3%83%BC%E3%82%B8%E3%83%A3%29+-+%E6%9D%B1%E5%8C%97%E5%A4%A7%E5%AD%A6%E3%82%B2%E3%83%BC%E3%83%A0%E5%88%B6%E4%BD%9C%E3%82%B5%E3%83%BC%E3%82%AF%E3%83%AB%0D%0A&related=micom_procedure"><img src="../assets/common/iconmonstr-twitter-4.svg"></a></li>
        <li><a href="https://www.facebook.com/sharer/sharer.php?u=https://sui828.github.io/micomprocedure/"><img src="../assets/common/iconmonstr-facebook-4.svg"></a></li>
        <li><a href="http://line.me/R/msg/text/?Micomprocedure%28%E3%83%9E%E3%82%A4%E3%82%B3%E3%83%B3%E3%83%97%E3%83%AD%E3%82%B7%E3%83%BC%E3%82%B8%E3%83%A3%29+-+%E6%9D%B1%E5%8C%97%E5%A4%A7%E5%AD%A6%E3%82%B2%E3%83%BC%E3%83%A0%E5%88%B6%E4%BD%9C%E3%82%B5%E3%83%BC%E3%82%AF%E3%83%AB%0D%0Ahttps%3A%2F%2Fsui828.github.io%2Fmicomprocedure%2F"><img src="../assets/common/iconmonstr-line-4.svg"></a></li>
      </ul>
    </div>
    <div class="copyright">&copy; Copyright micomprocedure 2021 all right reserved.</div>
  </footer>

    </div>
  </div>
</template>

<script>
import Carousel from '@/components/Carousel.vue'

export default {
  name: 'Top',
  data() {
    return {
      dialog1: false,
      dialog2: false,
      dialog3: false,
      dialog4: false,
      dialog5: false
    };
  },
  components: {
    Carousel
  },
  methods: {
    scrollTop: function(){
      window.scrollTo({
        top: 0,
        behavior: "smooth"
      });
    },
    scrollTop2: function(){
      window.scrollTo({
        top: 0,
      });
    },
    scrollAbout: function(){
      window.scrollTo({
        top: 700,
        behavior: "smooth"
      });
    },
    scrollWorks: function(){
      window.scrollTo({
        top: 1450,
        behavior: "smooth"
      });
    },
    scrollJoin: function(){
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
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
  @import "../assets/stylesheet.css"
</style>

<style lang="scss">

</style>