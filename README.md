# HoYoLAB Japanese Language Filter

## Overview

[HoYoLAB](https://www.hoyolab.com/home) の日本語フィルタを追加するためのChromeの拡張機能です。  
HoYoLABに投稿されたスレッドのうち、日本語による投稿のみを表示するための機能を提供します。  
2021年9月16日のHoYoLABのリニューアルに伴い以前は存在した言語フィルタが消滅したため、それに変わる代替手段として利用できます。  

本リポジトリは [suezu/hoyolab-language-filter](https://github.com/suezu/hoyolab-language-filter) のForkで、フィルタのON/OFF制御機能を追加しています（suezuさんに感謝！）。  

## Caution

[HoYoLABの利用規約](https://www.hoyolab.com/agreement) によるとプラグインの使用は規約違反的な記載があるので（利用規則の「許可されていない方法でmiHoYoサービスを使用する行為」に該当？）使用は自己責任にてお願いします。  

なおプラグインの拡散行為も規約違反の節があったり、オリジナルのプラグインのライセンス形態が現状不明瞭なので、本リポジトリ自体私の判断で突然削除する可能性もある旨ご理解ください。  

## Usage

### Filter Threads

拡張機能を追加するだけでHoYoLABの「ホーム」や「フォロー」、「ファンアート」内の日本語以外の投稿が非表示になります。  
なお拡張機能はストアには公開していないため、本リポジトリをCloneもしくはDLし直接追加ください。  

### Specification

「日本語の投稿」の定義は「タイトルに、ひらがな、カタカナ、もしくは漢字が含まれているか」です。  
よって「タイトルが英数字だけで記載された、本文にのみ日本語が含まれる投稿」は日本語の投稿とは判定されません。  
例えば「タイトル：Happy Birthday!、本文：お誕生日おめでとう！＜イラスト＞」のような投稿は非表示の対象となります。  

また「イチオシ」に認定された投稿は判定から除外されます。  
技術的には判定可能ですが、公式がイチオシに認定しているくらいなのだからそれは見えていても良いだろうという個人的な判断で、現状その部分には手を加えていません。  

### Disable Filter

拡張機能のポップアップ画面からフィルタのON/OFF設定が行なえます。  
フォローしているユーザに海外の方が多い、ファンアートでは海外の方の投稿も見たいというような方は必要に応じてフィルタをOFFに設定ください。  

![image](https://user-images.githubusercontent.com/57448478/133940359-c8a81eda-65ae-42c8-8b3b-99e4ae995e64.png)

なお「HoYoLabのページを開く → 別タブでもう一つHoYoLabのページを開いて設定を変更する → タブを切り替えて戻ってくる」と、設定の表示と内部の状態がズレるのでご理解ください。  
その場合、画面を更新すれば設定に合わせて状態がリセットされます。  
