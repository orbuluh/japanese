# MeCab

## Intro

MeCab 是一個開源的日本語形態素解析器，可以將日文句子進行詞彙切割、詞性標注、漢字音轉換等處理，提供了豐富的 API 和工具，可以方便地進行自然語言處理和文本分析。除了上面提到的詞性標注和動詞型判斷外，MeCab 還有以下功能：

分詞和標注：可以將日文句子進行詞彙切割和詞性標注，得到詞彙和詞性的列表，方便進行文本分析。

漢字音轉換：可以將漢字轉換為假名和拼音，方便進行音韻學研究和日語學習。

生成識別詞彙：可以利用已有的詞彙資料庫或文本資料，生成識別新詞彙的模型，方便進行新詞發現和詞彙擴充。

自定義詞彙：可以自定義詞彙，加入到詞彙資料庫中，方便進行特定領域的文本分析。

其他功能：MeCab 還支援通過 API 和命令行工具進行詞頻統計、命名實體識別、依存句法分析等處理，應用廣泛。

總之，MeCab 是一個功能強大的日本語形態素解析器，可以應用於文本分析、自然語言處理、語言學研究等領域，方便、快速地處理日語文本資料。

## Installation

```bash
sudo apt-get update
sudo apt-get install mecab libmecab-dev mecab-ipadic-utf8
pip install mecab-python3
```

## Error if ...

`[ifs] no such file or directory: /usr/local/etc/mecabrc`

```bash
mecab-config --sysconfdir
/etc

sudo mkdir -p /usr/local/etc
sudo ln -s /etc/mecabrc /usr/local/etc/mecabrc
```