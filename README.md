# google_scraping
Get Google search suggestions by scraping

## 今回の目的（Purpose）  
エキゾチックアニマルを飼うにあたり、どういった印象なのかを調べるためにGoogleの検索サジェストから簡単に取得しようと試みました。  
I did a quick search using Google's search suggestions to find out what people think about keeping an exotic animal.

## 概要（Overview）  
Google colaboratory環境にて、Googleの検索サジェストをスクレイピングにより取得する方法をご紹介します。  
インプット：Google spreadsheetの「Sheet1」シート  
アウトプット：Google spreadsheetの「結果」シート（「結果」シートをあらかじめ作成していなくて問題ないです。）  

In this article, we will introduce how to obtain Google search suggestions by scraping in a Google Colaboratory environment.  
Input: "Sheet1" sheet of a Google spreadsheet  
Output: "Results" sheet of a Google spreadsheet (It is okay if you have not created a "Results" sheet in advance.)  

「Sheet1」シートの内容は以下です。 

| animal_name           |
|------------------------|
| チンチラ               |
| フクロモモンガ         |
| シマリス               |
| フェレット             |
| モルモット             |
| ウサギ                 |
| ゴールデンハムスター   |
| リスザル               |
| セキセイインコ         |
| デグー                 |
| フェネック             |
| ショウガラゴ           |
| オカメインコ           |
| ハリネズミ             |
| ヒョウモントカゲモドキ |

The contents of "Sheet1" are as follows.  
| animal_name           |
|------------------------|
| Chinchilla             |
| Sugar Glider           |
| Chipmunk               |
| Ferret                 |
| Guinea Pig             |
| Rabbit                 |
| Golden Hamster         |
| Squirrel Monkey        |
| Budgerigar             |
| Degu                   |
| Fennec Fox             |
| Bush Baby              |
| Cockatiel              |
| Hedgehog               |
| Leopard Gecko          |

## フォルダ構成（Folder structure）  
Folder/  
├── Animal_scraping.ipynb               ← Google colaboratory用の実行ファイル（Executable file for google colaboratory）  
└── Exotic_animal        ← Google spreadsheetのファイル名（Google spreadsheet file name）  
