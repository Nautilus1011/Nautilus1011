<div align="center">

![header](https://capsule-render.vercel.app/api?type=waving&color=0:2E3192,100:1BFFFF&height=300&section=header&text=Nautilus1011&fontSize=90&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Software%20Engineer&descAlignY=55&descAlign=50)

</div>

<!-- 他のスタイルのヘッダー例（お好みで変更可能）

波型・グラデーション（現在使用中）:
![header](https://capsule-render.vercel.app/api?type=waving&color=0:2E3192,100:1BFFFF&height=300&section=header&text=Nautilus1011&fontSize=90&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Machine%20Learning%20Engineer&descAlignY=55&descAlign=50)

シャープな形・ブルー系:
![header](https://capsule-render.vercel.app/api?type=cylinder&color=0:83a4d4,100:b6fbff&height=250&section=header&text=Nautilus1011&fontSize=80&fontColor=ffffff&animation=twinkling)

シンプル・グラデーション:
![header](https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=0,2,3,5,6&height=250&section=header&text=Nautilus1011&fontSize=80&fontColor=ffffff&animation=fadeIn)

透明な波型:
![header](https://capsule-render.vercel.app/api?type=transparent&color=auto&height=250&section=header&text=Nautilus1011&fontSize=90&animation=scaleIn&fontAlignY=40)

-->


## 🚀 自己紹介
機械学習を軸に、開発環境の構築からアプリケーション開発まで幅広く取り組んでいます。
現在はコンピュータビジョンに興味があり、衛星画像解析とセグメンテーションタスクを研究しています。

## 💻 技術スタック

### プログラミング言語
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white)

### 開発環境・インフラ
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white)
<!-- 使っていれば追加
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Ubuntu](https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)
![uv](https://img.shields.io/badge/uv-DE5FE9?style=for-the-badge&logo=uv&logoColor=white)
-->

### 機械学習・コンピュータビジョン
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)
![YOLO](https://img.shields.io/badge/YOLO-00FFFF?style=for-the-badge&logo=yolo&logoColor=black)
![Hydra](https://img.shields.io/badge/Hydra-89b8cd?style=for-the-badge&logo=python&logoColor=white)
![TensorBoard](https://img.shields.io/badge/TensorBoard-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
<!--
![PyTorch Lightning](https://img.shields.io/badge/PyTorch_Lightning-792EE5?style=for-the-badge&logo=pytorchlightning&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
-->

### データ処理・可視化
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=for-the-badge&logo=python&logoColor=white)
![QGIS](https://img.shields.io/badge/QGIS-589632?style=for-the-badge&logo=qgis&logoColor=white)
<!--
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=for-the-badge&logo=python&logoColor=white)
-->

## 🎓 プロジェクト・研究活動

### 卒業研究：用途地域推定AIシステム
- 衛星画像を用いた用途地域の自動推定
- YOLOによる物体検出・セグメンテーション
- PyTorch、OpenCVなどを使用

### [lightning-ml-starter](https://github.com/Nautilus1011/lightning-ml-starter)
長期インターンで身につけた機械学習開発の進め方を、研究室のメンバーに共有するために作ったスターターテンプレートです。
Pascal VOCを題材に、Faster R-CNNによる物体検出の学習から推論までを一通り動かせます。

- **誰の環境でも同じように動く**: Docker / docker-composeで環境を固定しています。GPUがあれば使い、なければCPUで動きます。ホストとUIDを揃えた非rootユーザーで動かすので、生成ファイルの権限で困りません
- **実験を再現できる**: 設定はHydraでyaml 1つに集約し、コマンドラインから上書きできます。実行ごとの設定スナップショットとチェックポイントは日時別のディレクトリに保存し、学習の経過はW&Bで記録します
- **読みやすいコード構成**: PyTorch LightningのLightningModule / DataModuleでモデルとデータ処理を分け、学習と推論のエントリーポイントも分けています
- **初めての人でも追える**: Docker・Hydra・W&B・Lightning・argparseについて、実際のコードに沿った解説ドキュメントを用意しました。実行結果を残したNotebookもあり、手元で動かす前に全体の流れを確認できます
- **チーム開発の型**: Issue / PRテンプレートを用意し、ブランチを切ってPRでマージする流れで開発しています
- 使用技術: Python, PyTorch Lightning, Hydra, W&B, Docker

<!-- 
## 🚀 注目プロジェクト

### [プロジェクト名](https://github.com/Nautilus1011/repository-name)
**説明**: プロジェクトの簡単な説明をここに記載
- 🔹 特徴1
- 🔹 特徴2
- 🔹 使用技術: Python, PyTorch, OpenCV

### [プロジェクト名2](https://github.com/Nautilus1011/repository-name2)
**説明**: 別のプロジェクトの説明
- 🔹 特徴1
- 🔹 特徴2
- 🔹 使用技術: Python, Open3D

---

**または、GitHub Readme Statsを使ったカード形式での表示も可能です:**

<div align="center">
  <a href="https://github.com/Nautilus1011/repository-name">
    <img src="https://github-readme-stats.vercel.app/api/pin/?username=Nautilus1011&repo=repository-name&theme=tokyonight&hide_border=true" />
  </a>
  <a href="https://github.com/Nautilus1011/repository-name2">
    <img src="https://github-readme-stats.vercel.app/api/pin/?username=Nautilus1011&repo=repository-name2&theme=tokyonight&hide_border=true" />
  </a>
</div>
-->

<!-- 
## 📊 GitHub Stats

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Nautilus1011&show_icons=true&theme=tokyonight&hide_border=true" alt="GitHub Stats" height="170"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Nautilus1011&layout=compact&theme=tokyonight&hide_border=true" alt="Top Languages" height="170"/>
</div>

<div align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=Nautilus1011&theme=tokyonight&hide_border=true" alt="GitHub Streak" />
</div>
-->

## 🌱 現在学習中
- **Open3D**: 3次元点群データの処理と可視化
- **Transformer系ビジョンモデル**: ViT、DETRなど最先端のコンピュータビジョン技術
- **MLOps**: Dockerを使った実験環境の再現と、モデルデプロイメントパイプライン

## 📫 連絡先
- GitHub: [@Nautilus1011](https://github.com/Nautilus1011)

## ⚡ その他


---
<div align="center">
  <img src="https://komarev.com/ghpvc/?username=Nautilus1011&color=blue&style=flat-square" alt="Profile Views"/>
</div>
