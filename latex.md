## Latexの豆知識
### 図表関連
- 章ごとで分けるためには，以下をstyファイルに記載する
  - ```tex
    % 図番号を2.1のように章ごとで分ける
    \renewcommand{\thefigure}{
    \thesection.\arabic{figure}}
    \@addtoreset{figure}{section}
    % 表番号を2.1のように章ごとで分ける
    \renewcommand{\thetable}{
    \thesection.\arabic{table}}
    \@addtoreset{table}{section}
    % 数式を2.1のように章ごとで分ける
    \renewcommand{\theequation}{
    \thesection.\arabic{equation}}
    \@addtoreset{equation}{section}
    ```
- 図をカラーで出力するには，プリアンブルに以下を記述
  - ```tex
    \usepackage[dvipdfmx]{xcolor} %図をカラーで出力
    ```
- 図表の幅を指定する（2段組みでも適用可）
  - ```tex
    \includegraphics[width=\linewidth]
    ```
### 参考文献
- 参考文献にリンクを乗せるためのプリアンブル
  - ```tex
    \usepackage{hyperref} %参考文献のリンクの体裁用
    \usepackage{breakurl}
    ```
- 参考文献を順番に並べる
  - ```tex
    \bibliographystyle{junsrt}　% 参考文献を順番に
    ```
### 細かいこと
- 「～」は
  - ```tex
    $\sim$
    ```
- 複数章がある場合は
  - ```tex
    \input{include/chap1}
    ```
