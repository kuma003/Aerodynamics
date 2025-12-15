# Aerodynamics
14期代空力班の引継ぎ資料

# ファイル
引継ぎ資料は以下の4つから構成されます．  
このうち，英訳版についてはAIによる翻訳なので参考程度に見てください．

- [【メイン資料】空気力学の基礎 (仮称)](docs/aero.pdf)
- [【メイン資料 (英訳版)】Fundamentals of Aerodynamics (仮称)](docs/aero_en.pdf)  
- [【補助資料】減衰モーメント係数について](docs/damping_moment.pdf)
- [【補助資料】壁面粗さと壁面y+値について](docs/wall_function.pdf)


# 改訂者へ
全てLaTex (upLaTex) で作成しています．
また，VS Code上でLatex Workshopを用いて執筆するのを想定しています．
この場合，保存時に自動でビルドし，生成ファイルがdocsディレクトリに出力されます ([settings.json](.vscode/settings.json)参照) ．

LaTexの環境構築については各自調べて導入にしてください．
未検証ですが環境構築が手間な場合は [Overleaf](https://www.overleaf.com/) でも編集できると思います．

可能ならこのrepositoryをforkしてから修正するのを推奨します．
この場合，pull requestを送ってくれたら対応します（気付いていない場合はご連絡ください）．

以下に，大まかな手順等を紹介します．
### 1. ウェブページでの作業①
1. githubのアカウントを作成する
2. [このページ](https://github.com/kuma003/Aerodynamics.git) の右上にあるForkボタンから，このリポジトリをforkします
3. 自身のforkしたリポジトリで右上緑色のCodeボタンをクリックし，`https://github.com/(username)/Aerodynamics.git` のようなURLを確認してコピーします

### 2. ローカルでの作業
1. コマンドプロンプト (or PowerShell) を開く
2. `cd (保存先のディレクトリのパス)`でカレントディレクトリを変更する
 (1, 2については，ファイルエクスプローラで保存先のディレクトリを開き，上のパスが表示される小窓に`cmd`と入力してもokです)
3. `git clone https://github.com/(username)/Aerodynamics.git` でファイルをコピー
4. `cd Aerodynamics` で移動
5. 編集する.  Overleafを使うなら，編集後適宜texファイルやpdfを更新する．
6. 以下のコマンドで変更したファイルを全部コミット・プッシュ
 ```
 git add (変更したファイルパス，面倒なら . (ピリオド)で変更したファイル全指定) 
 git commit -m (コミットメッセージ)
 git push
 ```

### 3. ウェブページでの作業②
1. 自分のリポジトリを開き，左上のボタンからPull requestsのページに飛びます．
2. New pull requestから，pull requestを作成して送信します．タイトルや説明文は任意です．

以上で終わりです．




今後も内容が精査・修正され，適切に知識が継承・発展されていくことを願ってやみません．

