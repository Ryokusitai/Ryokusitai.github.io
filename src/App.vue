<script setup>
import { useDark } from '@vueuse/core';
import { ref } from 'vue';

import Avatar from './assets/mooncitymountains.jpg';
import PEAA from './assets/peaa.png';
import OldMassFabricator from './assets/OldMassFabricator.png';
import OldMassFabricatorRecipe from './assets/OldMassFabricator_Recipe.png';

useDark();

const activeName = ref('1.7.10');
const dialogVisible = ref(false);
</script>

<template>
  <el-container style="max-width: 1140px; margin: 0 auto;">
    <el-main>
      <el-card>
        <div style="display: flex;">
          <el-avatar :src="Avatar" :size="100" fit="cover" shape="square"></el-avatar>
          <div style="calc(100% - 100px); padding-left: 2em;">
            <h2 style="margin: 0;">
              Author: ryokusitai
              <el-link href="https://github.com/Ryokusitai" target="_blank" :underline="false"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16" width="16" height="16" style="fill: currentColor;"><path d="M8 0c4.42 0 8 3.58 8 8a8.013 8.013 0 0 1-5.45 7.59c-.4.08-.55-.17-.55-.38 0-.27.01-1.13.01-2.2 0-.75-.25-1.23-.54-1.48 1.78-.2 3.65-.88 3.65-3.95 0-.88-.31-1.59-.82-2.15.08-.2.36-1.02-.08-2.12 0 0-.67-.22-2.2.82-.64-.18-1.32-.27-2-.27-.68 0-1.36.09-2 .27-1.53-1.03-2.2-.82-2.2-.82-.44 1.1-.16 1.92-.08 2.12-.51.56-.82 1.28-.82 2.15 0 3.06 1.86 3.75 3.64 3.95-.23.2-.44.55-.51 1.07-.46.21-1.61.55-2.33-.66-.15-.24-.6-.83-1.23-.82-.67.01-.27.38.01.53.34.19.73.9.82 1.13.16.45.68 1.31 2.69.94 0 .67.01 1.3.01 1.49 0 .21-.15.45-.55.38A7.995 7.995 0 0 1 0 8c0-4.42 3.58-8 8-8Z"></path></svg></el-link>
              <el-link href="https://twitter.com/ryokusitai_mod" target="_blank" :underline="false"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="16" height="16" data-name="Layer 1" id="twitter" style="fill: currentColor;"><path d="M22,5.8a8.49,8.49,0,0,1-2.36.64,4.13,4.13,0,0,0,1.81-2.27,8.21,8.21,0,0,1-2.61,1,4.1,4.1,0,0,0-7,3.74A11.64,11.64,0,0,1,3.39,4.62a4.16,4.16,0,0,0-.55,2.07A4.09,4.09,0,0,0,4.66,10.1,4.05,4.05,0,0,1,2.8,9.59v.05a4.1,4.1,0,0,0,3.3,4A3.93,3.93,0,0,1,5,13.81a4.9,4.9,0,0,1-.77-.07,4.11,4.11,0,0,0,3.83,2.84A8.22,8.22,0,0,1,3,18.34a7.93,7.93,0,0,1-1-.06,11.57,11.57,0,0,0,6.29,1.85A11.59,11.59,0,0,0,20,8.45c0-.17,0-.35,0-.53A8.43,8.43,0,0,0,22,5.8Z"/></svg></el-link>
            </h2>
            <hr style="margin-top: 0;">
            <div>Java,C#,Vue</div>
            <div>homebody</div>
          </div>
        </div>
      </el-card>
      <h2>Mods（<el-link type="primary" @click="dialogVisible = true">利用規約・謝辞など</el-link> ）</h2>
      <el-tabs type="border-card" v-model="activeName">
        <el-tab-pane label="MC1.7.10" name="1.7.10">
          <el-tabs class="tab-mods" tabPosition="left">
            <!-- PEAA -->
            <el-tab-pane label="PEAA">
              <div style="height: 100%; overflow-y: auto;">
                <el-image :src="PEAA" />
                <p>A.K.さんがMinecraft1.2.5にて開発していらしたEE2のアドオンである <el-link href="https://web.archive.org/web/20190715143042/https://forum.minecraftuser.jp/viewtopic.php?f=13&t=6672&start=500#p127945" target="_blank" type="primary">EEAA(EE2Addon Advanced Alchemy)</el-link> 
をProjectE1.7.10 環境に対応させたものです。<br>A.K.さんが開発を再開するまでという条件付ではありますが、A.K.さんから公式に許可を頂いております。</p>
                <h3 style="border-bottom: solid 1px;">使い方（WIP）</h3>
                <p>いつか書きます</p>
                <h3 style="border-bottom: solid 1px;">ダウンロード</h3>
                <p>ProjectE-1.8.0以降：<el-link href="https://www.dropbox.com/sh/rns7170f4jsf3l1/AABJF9adY8KuiGq2hXERFbDIa/PEAA-1.5.4.jar?dl=0" target="_blank" type="primary">PEAA-1.5.4</el-link></p>
                <p>ProjectE-1.1.0以前：<el-link href="https://www.dropbox.com/sh/rns7170f4jsf3l1/AACZgKiERb6mzoH4qu-YQR5Ea/PEAA-1.3.3.jar?dl=0" target="_blank" type="primary">PEAA-1.3.3</el-link></p>
                <h3 style="border-bottom: solid 1px;">ダウンロード（オプション）</h3>
                <p>
                  <span>旧テクスチャ（トップ画像右下のやつ）：</span><el-link href="https://www.dropbox.com/sh/rns7170f4jsf3l1/AADvHLf9OFRyBxOC8vnbCyzIa/oldTextures.zip?dl=0" target="_blank" type="primary">OldTexture</el-link>
                  <span style="display: inline-block; margin-left: .5em; padding-left: .25em; border-left: solid 1px;">
                    modのjarファイルを一度展開してから中のテクスチャをダウンロードした旧テクスチャに置き換え。その後再度jarにして使用する必要があります。ちょっと大変かもしれないです。
                  </span>
                </p>
              </div>
            </el-tab-pane>
            <!-- EREMC -->
            <el-tab-pane label="EREMC">
              <div style="height: 100%; overflow-y: auto;">
                <p>PEAA1.2.1までの「ic2ex」「BuildCraft」の一部のアイテムにEMCが追加登録される機能を別MOD化したものです。<br>このMODの動作にPEAAは不要です</p>
                <h3 style="border-bottom: solid 1px;">使い方（WIP）</h3>
                <p>導入するだけで自動でEMCが設定されます</p>
                <h3 style="border-bottom: solid 1px;">ダウンロード</h3>
                <p>ProjectE-1.2.0以降：<el-link href="https://www.dropbox.com/sh/rns7170f4jsf3l1/AAC5NAaXDjg_-WPhW0ly5aiPa/EREMC-1.3.0.jar?dl=0" target="_blank" type="primary">EREMC-1.3.0</el-link></p>
              </div>
            </el-tab-pane>
            <el-tab-pane label="OldMassFabricator">
              <div style="height: 100%; overflow-y: auto;">
                <el-image :src="OldMassFabricator" />
                <p>旧仕様(ic2仕様)の固体マター製造機を追加します。</p>
                <h3 style="border-bottom: solid 1px;">使い方</h3>
                <p>上下からスクラップ及びスクラップボックスの搬入が、横からはマターの搬出が出来ます。<br/>
レンチを使えば100%回収できます。つるはしなどで破壊した場合、他の機械のようにマシンケーシングになってしまいます。<br/>
マターを使って作れるレシピも旧仕様と同じになってるはずです。<br/>
のと氏の <el-link href="https://web.archive.org/web/20190715144859/http://forum.minecraftuser.jp/viewtopic.php?f=13&t=5440" target="_blank" type="primary">「SolidMatter+」</el-link>のマターと相互変換が可能です</p>
                <h3 style="border-bottom: solid 1px;">クラフトレシピ</h3>
                <el-image :src="OldMassFabricatorRecipe" />
                <p>現在のマター製造機と時計です(不定形レシピ)。将来的にレシピが変更になる可能性があります。</p>
                <h3 style="border-bottom: solid 1px;">ダウンロード</h3>
                <p><el-link href="https://www.dropbox.com/sh/rns7170f4jsf3l1/AAD-V3Kzo46rbMuDmutV5ZYDa/oldMassFabricator-1.1.4.jar?dl=0" target="_blank" type="primary">OldMassFabricator-1.1.4</el-link></p>
                <h3 style="border-bottom: solid 1px;">謝辞</h3>
                <p>MinecraftModdingWikiの解説及び、A.K.さんが公開してくださっている
「永久光発電機MOD(VisibleRayGenerator)」のソースコードがなければ
このMODは完成しませんでした。また、defeatedcrow氏が公開してくださっている
AppleMilkTea version2のソースコードも非常に参考になりました。どうも有難うございます。</p>                
              </div>
            </el-tab-pane>
          </el-tabs>
        </el-tab-pane>
        <el-tab-pane label="MC1.16.5(まだない)" name="1.16.5" disabled>Not Yet</el-tab-pane>
        <el-tab-pane label="MC1.20.0(まだない)" name="1.20.0" disabled>Not Yet</el-tab-pane>
      </el-tabs>
    </el-main>
  </el-container>

  <el-dialog v-model="dialogVisible" title="いろいろ">
    <h2 style="margin-top: 0;">利用規約</h2>
    <p>ここで公開されているMODは<el-link href="http://tsoft-web.com/nokiyen/minecraft/modding/MMPL_J" target="_blank" type="primary">「MMPL_J」</el-link>の元で配布されています。
この範囲内であれば連絡なく許諾されます。
Modpackの作成についても制限しません。ご自由にどうぞ。
ここで公開されているMODを利用(Modpack経由での利用を含む)した際に如何なる問題や障害が生じても、私は一切責任を負いません。
あらかじめご了承ください。</p>
      <h2>謝辞</h2>
      <p>MODを作成するに当たり、MinecraftModdingWikiには大変お世話になりました。<br/>
また、ASMライブラリの利用やIC2、BCなどのブロックを参照する方法、テレポート処理など
さまざまなものに関して、<el-link href="https://web.archive.org/web/20190715144859/http://forum.minecraftuser.jp/viewtopic.php?f=13&t=6672" target="_blank" type="primary">「A.K.さん」</el-link>が公開してくださっているソースコードが<br/>
パケット処理やGui, TileEntity, Configの利用方法などにおいてsinkillerjさんが公開してくださっているProjectEのソースコード非常に参考になりました。
どうも有り難うございました。</p>
      <h2>全部のMODの置き場所</h2>
      <el-link href="https://www.dropbox.com/sh/rns7170f4jsf3l1/AAAQ2TvfMg6_0GoiJASeVONIa?dl=0" target="_blank" type="primary">「このDropBox」</el-link>です。
      <h2>旧フォーラムの僕のページ(のWebアーカイブ)</h2>
      <el-link href="https://web.archive.org/web/20190715144859/https://forum.minecraftuser.jp/viewtopic.php?f=13&t=24695" target="_blank" type="primary">「ここ」</el-link>です。
  </el-dialog>
</template>

<style scoped>
.el-container {
  --tab-height: 60vh;
}
.el-tabs.tab-mods {
  height: var(--tab-height);
}
.el-tabs.tab-mods .el-tab-pane {
  height: var(--tab-height);
}
.el-link {
  vertical-align: baseline !important;
}
</style>
