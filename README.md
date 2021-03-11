# README
## 1. マイドライブに学習済みモデルやconfigファイルを配置
- [BERT with SentencePiece を日本語 Wikipedia で学習してモデルを公開しました](https://yoheikikuta.github.io/bert-japanese/)からダウンロード。
    - wiki-ja.*: SentencePieceの学習済みモデル。
    - model.ckpt-1400000.*: SentencePiece+BERTで学習済みモデル。
    - これらをマイドライブの研究/sentencepiece+bertディレクトリに配置すると仮定(ディレクトリがなければ作成)。
- [bert_config.json](./bert_config.json) を準備。
    - ここでは前述の学習済みモデルと同じディレクトリに保存すると仮定。

## 2. データセットの準備
- 今回用いるデータセットは指導教員である當間先生が管理しているため、當間先生から受け取る。
- これらをマイドライブの研究/ver-20200312ディレクトリにcsv形式で配置すると仮定。


## 3. 実験のソースコードの配置・実行
- [本実験.ipynb](./本実験.ipynb) と[基礎実験.ipynb](./基礎実験.ipynb)をダウンロードし、マイドライブに配置すると仮定。
- これらをgoogle colaboratoryで開き、上記のメニューバーから[ランタイム]→[ランタイムのタイプを変更]を選択し、ハードウェアアクセラレータがNoneになっている箇所をGPUに変更。
- 上記のセルから順序よく実行。
