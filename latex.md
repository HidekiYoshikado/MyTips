## Latexの豆知識
### 図表関連
- ```tex
  \renewcommand{\thefigure}{% 図番号の付け方
  \thesection.\arabic{figure}}
  \@addtoreset{figure}{section}
  ```
- ```tex
  \renewcommand{\thetable}{% 図番号の付け方
  \thesection.\arabic{table}}
  \@addtoreset{table}{section}
  ```
