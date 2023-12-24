---
marp: true
theme: satooru-mocopi
paginate: true
class: lead
math: mathjax
---

<!--
_class: gaia lead
_paginate: false
-->

# センシング と mocopi

来年の目標にセンシングはどうですか？

<br>

愛知工業大学 システム工学研究会
B1 多田 隆人

---

<!-- _header: だれ -->

<img
   src="images/broken_penguin.png"
   width="400"
   style="
      position:fixed;
      top: 230px;
      left: 160px;
   "
/>

<div style="margin-left:570px">

   - 名電 情報科 (2023年卒)
   - 元 情シス部長
   - ぺんぎんがすき　

</div>

---

## センシングとは

---

<!-- header: センシングとは -->
<!-- class: lead -->

### 様々な情報を計測してデータ化すること

<div style="margin-left:390px">

- 万歩計
- ポケモン GO
- カーナビ etc.

</div>

日常の至る所で使われている

---

<!-- header: "" -->
<!-- _class: gaia lead -->

# センシング x mocopi

---

<iframe
   src="https://www.youtube.com/embed/g0d-x0l2HtA?si=XaV0OP78yE2_MYJ2&amp;start=100"
   frameborder="0"
   allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
   allowfullscreen
></iframe>

---

<iframe
   src="https://www.youtube.com/embed/s0G8u1el42g?si=HG-GdQhORp0Ll5iC&amp;start=129"
   title="YouTube video player"
   frameborder="0"
   allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
   allowfullscreen
></iframe>

---

<!-- header: "" -->

### どこまでできる？
辰巳先生）mocopiで野球のデータ分析をやりたい

---

<!-- header: mocopi の精度 -->

### 腕を上げる
<iframe
   src="https://www.youtube.com/embed/QXMYon2XJrY"
   frameborder="0"
   allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
   allowfullscreen
></iframe>

---

<iframe
   src="https://www.youtube.com/embed/ozdsx7HVQww?si=M6v-_RfOUvfzBsxV" 
   title="YouTube video player"
   frameborder="0"
   allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
   allowfullscreen
></iframe>

---

<p style="font-size:1.5rem">(Pythonで簡単に触れるパッケージを自作してたり...)<p>
<img
   src="images/walk_square.png"
   width="100%"
/>

スタート地点とゴール地点がずれた！

---

センサーには必ず誤差がある
最悪だね

<div class="arrow middle"></div>

**このデータをどう扱えば良い？**

---

<iframe
   src="https://www.youtube.com/embed/NtCvLE0HBFA"
   title="歩行推定 高大連携LT会用"
   frameborder="0"
   allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
   allowfullscreen
></iframe>

---

<!-- header: 歩数推定してみる -->

<img
   src="images/acc.png"
   width="100%"
/>

<div class="arrow middle"></div>

この加速度から歩数を出してみる

---


<img
   src="images/acc3.png"
   width="100%"
/>

必要な部分を切り出す

---


<img
   src="images/acc4.png"
   width="100%"
/>

ノルムに変換する ($norm = \sqrt{x^2 + y^2 + z^2}$)

---

<img
   src="images/acc5.png"
   width="100%"
/>

滑らかにする(平滑化フィルタ)

---

<!-- _header: 歩数を出してみる -->

<img
   src="images/acc7.png"
   width="100%"
/>

うまくいった 😊

---

<!-- _header: これから -->
<!-- _class: center -->

#### mocopiを使って<br>ある動作から積み重なった誤差を減らす研究をしたい

<div style="margin-left:70px">

例)
　歩くと必ず足が伸びるタイミングがある
　　↓
　常に曲がっていたらまっすぐになるように補正

</div>

---

<!-- _header: まとめ -->

1. センシングは現実世界の情報をデータ化できる
2. データは必ず誤差を含む
3. データをどう扱うかが重要
4. 今後にセンシングはどうですか？
