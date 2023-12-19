---
marp: true
theme: satooru-mocopi
paginate: true
class: lead
---

<!--
_class: gaia lead
_paginate: false
-->

# センシング と mocopi

今後の人生にセンシングはどうですか？

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

<!-- _header: センシングとは -->

### 様々な情報を計測してデータ化すること

---

TODO: 歩いている様子の動画

---

<!-- _header: 歩行をセンシング -->
<!-- _class:  -->

### 歩いている様子を計測

TODO: 加速度のグラフ

---

<!-- _header: 歩数を出してみる -->

TODO: 歩数をプロットしたグラフ

正しく歩数を出せていない

<div class="arrow middle"></div>

データを整形してみる

---

<!-- _header: 歩数を出してみる -->

TODO: 歩数をプロットしたグラフ with 平滑化フィルタ

うまくいった 😊

---

### センシング x mocopi

---

TODO: VRChat している様子の動画

---

<!-- _header: mocopi の精度 -->

### 腕を上げる
TODO

---

<!-- _header: mocopi の精度 -->

### ジャンプする
TODO

---

<!-- _header: mocopi の精度 -->

### 移動する
TODO

---

<!-- _header: mocopi の精度 -->

### 長時間動く
TODO

---

<!-- _header: mocopi の精度 -->

最悪だね
センサーには必ず誤差がある

<div class="arrow middle"></div>

**このデータをどう扱えば良い？**

---

<!-- _header: "例: ~TODO~" -->

### 

---

...

---

<!-- _header: これから -->
<!-- _class: center -->

#### mocopiを使って<br>ある動作から積み重なった誤差を減らす研究をしたい

例)
　歩くと必ず足が伸びるタイミングがある
　　↓
　常に曲がっていたらまっすぐになるように補正

---

<!-- _header: まとめ -->

1. センシングは現実世界の情報をデータ化できる
2. データは必ず誤差を含む
3. データをどう扱うかが重要
4. 今後にセンシングはどうですか？
