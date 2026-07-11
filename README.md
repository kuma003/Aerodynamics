# Aerodynamics

14期代空力班の引継ぎ資料です．

## 資料

- [【メイン資料】空気力学の基礎（仮称）](https://kuma003.github.io/Aerodynamics/aero.pdf)
- [【メイン資料・英訳版】Fundamentals of Aerodynamics](https://kuma003.github.io/Aerodynamics/aero_en.pdf)
- [【補助資料】Barrowman Methodを用いた解析について](https://kuma003.github.io/Aerodynamics/Barrowman_method.pdf)
- [【補助資料】減衰モーメント係数について](https://kuma003.github.io/Aerodynamics/damping_moment.pdf)
- [【補助資料】壁面粗さと壁面y+値について](https://kuma003.github.io/Aerodynamics/wall_function.pdf)

英訳版はAIによる翻訳を含むため，参考資料として利用してください．

## PDFの公開

`main` ブランチへpushすると，GitHub Actionsが全資料をビルドし，[GitHub Pages](https://kuma003.github.io/Aerodynamics/)へ公開します．生成されたPDFは，Actionsの `aerodynamics-pdfs` artifactからも90日間ダウンロードできます．

PDF本体とLaTeXの補助ファイルはGitで管理しません．ソースの `.tex`，参考文献，画像など，文書の生成に必要なファイルだけをコミットしてください．

## 改訂方法

各資料はupLaTeXで作成しています．VS CodeとLaTeX Workshopを使う場合，保存時に自動ビルドされ，生成物は `docs` ディレクトリへ出力されます．設定の詳細は [.vscode/settings.json](.vscode/settings.json) を参照してください．

ローカルにLaTeX環境を用意できない場合は [Overleaf](https://www.overleaf.com/) も利用できますが，本リポジトリの構成での動作は未検証です．

変更を提案する場合は，このリポジトリをforkしてPull Requestを送る方法を推奨します．

### 1. リポジトリをforkする

1. GitHubアカウントを作成します．
2. [このリポジトリ](https://github.com/kuma003/Aerodynamics)を開き，右上の「Fork」から自分のアカウントへforkします．
3. fork先の「Code」からURLをコピーします．URLは `https://github.com/<username>/Aerodynamics.git` の形式です．

### 2. ローカルで編集する

```console
git clone https://github.com/<username>/Aerodynamics.git
cd Aerodynamics
```

編集後は，意図した変更だけをステージしてコミットします．

```console
git add <変更したファイル>
git commit -m "変更内容を表すメッセージ"
git push
```

### 3. Pull Requestを作成する

fork先の「Pull requests」から「New pull request」を選び，変更内容と理由を記載して送信してください．

今後も内容が精査・修正され，知識が適切に継承・発展されていくことを願っています．
