<p><H3>オールウェーブ DSPラジオIC SI4732をPi Picoで制御する</H3></p>
<p>
GitHubにあるSI4732の<a href="https://github.com/pu2clr/SI4735">ライブラリ</a>には、Pi PicoでSI4732を制御することができるとあり、"example"に例がある。<br>
ここでは、機能的に完結しているArduino Pro mini対応の"SI47XX_02_ALL_IN_ONE_OLED"をPi Pico用に改修した例を示す。<br>
開発はArduino IDE 2.1で行った。<br>
</p>

<p><strong>概要</strong><br>
改修前のスケッチでは、操作をボタンとロータリーエンコーダーで行っている。これは、このまま変更しないことにする。I2Cとリセットのピンは変更する。<br>
なお、回路（"schematic2.pdf"）としては、SI4732のオーディオ出力不足を補うためと感度向上のため、オペアンプの増幅回路（ローパスフィルタ付）と<br>
トランジスタの高周波増幅回路を追加している。<br>
実装については基板（PCB）化を行った。<br>
</p>
<p><strong>H/W構成</strong><br>
 ・Raspberry Pi Pico - コントローラ<br>
 ・I2C接続&nbsp; SI4732<br>
 ・I2C接続&nbsp; OLED表示装置(SSD1306)<br>
 ・ボタンとロータリーエンコーダー<br>
 ・オペアンプ NJM4580<br>
 ・高周波増幅 トランジスタ S9018<br>
 ・Xtal発振器（32768Hz）、抵抗・コンデンサ類、オーディオジャック、配線類<br>
</p>
<p>
<img src="./SI4732_Pi_Pico_1.jpg" width="480" height="360"><br>
</p>
<p><strong>接続</strong><br>
各コンポーネントの接続は以下の通り。<br>
<p>
<table> 
<tr>
<td>I2C&nbsp;</td><td>Pi_Pico</td>
</tr>
<tr>
<td>SDA(SI4732,OLED)</td><td>20</td>
</tr>
<tr>
<td>SCK(SI4732,OLED)</td><td>21</td>
</tr>
<tr>
<td>RESET(SI4732)</td><td>22</td>
</tr>
</table>
</p>
*その他の接続については、スケッチを参照のこと<br>
**プルアップ抵抗は省略可<br>
</p>
<p><strong>インストール</strong><br>
<ol>
<li>コードを、ZIP形式でダウンロード</li>
<li>追加のライブラリを、ZIP形式でダウンロード又はライブラリマネージャからインストールする</li>
 <ul>
  <li>SI4735（ライブラリマネージャから検索可）</li>
  <li>Tiny4kOLED（ライブラリマネージャから検索可）</li>
 </ul>
<li>ArduinoIDEからSI47XX_02_ALL_IN_ONE_OLED_pi_pico_master.inoを開く</li>
<li>「検証・コンパイル」に成功したら、一旦、「名前を付けて保存」を行う</li>
</ol>
</p>
<p><strong>若干の解説</strong><br>
・STEPのボタン（エンコーダに接続）は、FM受信中は周波数のプリセット（変数"fmstation[] "に定義）切り替えとして動作する。<br>
・電源を入れるとPi PicoのLEDが点灯する。<br>
・変数"Band band[]"の４番目の定数は、バンド切り替え時の既定の受信周波数である。地域の放送局に合わせると良い。<br>
<p>
<img src="./SI4732_Pi_Pico_2.jpg" width="540" height="360"><br>
</p>
</p>
<p><strong>注意事項</strong><br>
・利用の際は、自己責任でお楽しみください。<br>
</p>
