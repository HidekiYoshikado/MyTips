## pythonのvenvの使い方
- python3.3以降使用可能
### コード各種
- 仮想環境の作成
  - ```
    python -m venv [newenvname]
    ```
  - こうすると，実行パス直下に[newenvname]のフォルダが生成される
- 仮想環境に入る
  - windowsの場合
    - ```bash
      .\[newenvname]\Scripts\activate
      ```
  - ubuntuの場合
    - ```bash
      source [newenvname]/bin/activate
      ```
- 仮想環境から出る
  - ```bash 
    ([newenvname])$ deactivate
    ```
  
     
