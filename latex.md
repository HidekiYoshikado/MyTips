## Latexの豆知識
### 図表関連
章ごとで分けるためには，以下をstyファイルに記載する
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
