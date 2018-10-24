# Tic-Tac-Toe
用Python实现一个井字棋小游戏<br>
井字棋是一种小游戏，两位玩家轮流在3*3矩阵中标上X和O，先将3颗棋子连成水平，垂直或对角线者获胜。<br>
&nbsp;&nbsp;&nbsp;&nbsp;1 &nbsp;&nbsp;&nbsp;&nbsp;2&nbsp; &nbsp;&nbsp;&nbsp;3<br>
1&nbsp;&nbsp;X &nbsp;&nbsp;&nbsp;&nbsp;. &nbsp;&nbsp;&nbsp;&nbsp;.<br>
2&nbsp;&nbsp;&nbsp;&nbsp;. &nbsp;&nbsp;&nbsp;X &nbsp;&nbsp;&nbsp;.<br>
3&nbsp;&nbsp;&nbsp;&nbsp;. &nbsp;&nbsp;&nbsp;. &nbsp;&nbsp;&nbsp;&nbsp;X<br>
在游戏中，用 `'.'` 表示空棋盘，用`'X'`，`'O'`分别表示两玩家，每落一个子刷新显示棋盘，直到一方获胜或者棋盘已满。<br>
## 游戏规则：<br>
1.如果是第三步，且对手第二步下在边上，就下在中央。（这是特殊规则）<br>
2.如果存在可以立即获胜的位置，就下在这个位置。<br>
3.如果存在可以让对手立即获胜的位置，就下在这个位置。<br>
4.如果上面两种情况都不存在，但存在可以形成双二的位置，就下在这个位置。<br>
5.否则，下在优先列表中第一个可下的位置。（其中优先列表为pref_list=[1,9,3,7,5,2,4,6,8]）<br>
