# アスペクトを考慮した日本語時間推論データセットの構築（Jamp_sp: Controlled Japanese Temporal Inference Dataset Considering Aspect）

## Jamp_sp および当リポジトリについて

**Jamp_sp** は日本語の時間推論ベンチマークです。
このリポジトリはJamp_spを公開したもので、次のような構成になっています。末尾に _wakati がついたファイルはついていないファイル中の文章を分かち書きしたものです。

```
- dataset
  - template/tmeplate_ver_2_2.tsv: 時間推論テンプレート
  - test_2.tsv: テストデータ
  - train_all.tsv: 学習データ
  - train_custom_*.tsv: 分割後の学習データ（分割について詳しくは下に示す論文を参照）
    - train_custom_template-{easy/hard}.tsv: テンス現象タグをもとに分割を行ったもの
    - train_custom_timeformat-{easy/hard}.tsv: 時間表現形式をもとに分割を行ったもの
    - train_custom_timespan.tsv: タイムスパンをもとに分割を行ったもの
```

## About Jamp_sp and this repository

**Jamp_sp** is the Japanese temporal inference benchmark. This repository consists of templates, test data, and training data. The test data and training data both include tokenized and non-tokenized data. Tokenized data contains `wakati` in the file names. The training data contains both non-split data that includes all problems and split data following the methodology described in the paper. Files containing `template`, `time format`, or `time span` in their names are split based on **tense fragment**, **time format**, or **time span**, respectively.


## Citation

このデータセットを使用する場合は以下を引用してください。

```
@article{Sugimoto-jampsp-2023,
  title={アスペクトを考慮した日本語時間推論データセットの構築},
  author={杉本 智紀 and 尾上 康雅 and 谷中 瞳},
  journal={自然言語処理},
  volume={31},
  number={2},
  pages={-},
  year={2024},
  doi={}
}
```

If you use this dataset in any published research, please cite the following:

```
@article{Sugimoto-jampsp-2023,
  title={Jamp_sp: Controlled Japanese Temporal Inference Dataset Considering Aspect},
  author={Sugimoto, Tomoki  and
      Onoe, Yasumasa  and
      Yanaka, Hitomi},
  journal={Journal of Natural Language Processing},
  volume={31},
  number={2},
  pages={-},
  year={2024},
  doi={}
}
```


## Contact

質問や問題があれば、sugitomo555@gmail.com までお願いします。

For questions and usage issues, please contact sugitomo555@gmail.com

## License

- [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)