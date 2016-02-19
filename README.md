# 縦書き tumblr テーマ『長雨』

tumblr で利用できる縦スクロール型の縦書きテーマ。Safari, Chrome, Opera, Firefox, IE10+, Edge 対応

デモ [nagame-theme.tumblr.com](http://nagame-theme.tumblr.com)

## 概要

日本語縦書きに適したテーマです。web 上で縦書きを実現する技術は当初 Safari や Google Chrome など Webkit 系のブラウザに実装され、のち Internet Explorer や Firefox にも導入されました。この縦書きテーマ『長雨（ながめ）』を使用すると、主要なモダンブラウザ上で縦書き表示を実現することができます（IE は10以上が必要）。

実験的な追加機能として、Webフォント（旧字明朝体フォント『[馬酔木明朝](https://metasta.github.io/asebi/)』）もオプションで使用可能です。

## 使用法

 1. [nagame-theme.html](https://raw.githubusercontent.com/metasta/nagame/master/nagame-theme.html) の内容を全選択・コピーする
 2. tumblr のテーマカスタマイズ画面を開き「html を編集」をクリック
 3. 元の html を消去して nagame-theme.html をペースト

## カスタマイズ（テーマ編集画面から）

- タイトル・説明文・プロフィール画像の表示の有無
- テキストの色（デフォルト: #222）
- 使用フォント（游明朝体(YuMin) or 旧字明朝体フォント 馬酔木明朝(Asebi)）
- 段組の高さ（デフォルト：26字）

## 使用に際して

### 旧字について

- 新字／旧字表記をフォントで指定できる。以下の3通りの方法がある。
    1. 全ての投稿に新字／旧字を指定: 上記のカスタマイズ画面から
    2. 個々の投稿に新字／旧字を指定: 投稿のさい以下のキーワードをタグとして追加する
        - 新字: `newfont`、`modern`、`shinji` のどれか
        - 旧字: `oldfont`、`trad`、`classical`、`kyuji`のどれか
    3. 文章の一部に新字／旧字を指定: 表記を変更したい範囲を直接 html タグで指定（tumblr の投稿には html タグを含めることができる）

             新字で表記された文章の<span class="kyuji">一部分だけを旧字に変更</span>する
             旧字で表記された文章の<span class="shinji">一部分だけを新字に変更</span>する

- 以下の漢字はフォントだけでは旧表記が実現できないので、判断して正しい字を入力する必要がある。
    - 2つ以上の旧字をもつ「欠（缺）」「弁（瓣辯辨）」「予（豫）」「余（餘）」([このページ](https://metasta.github.io/asebi/annex/note.html) にメモをまとめた)、加えて「芸（藝）」も
    - 「画（劃）」「技量（伎倆）」「知恵（智慧）」「包帯（繃帯）」など「[同音の漢字による書きかえ](http://kokugo.bunka.go.jp/kokugo_nihongo/joho/kakuki/03/bukai03/03.html)」の対象となった字や語

### ルビについて

- tumblr の投稿には html タグを記述できるため、以下の記法でルビをふることができる。

             <ruby>縦<rt>たて</rt>書<rt>が</rt></ruby>き
             <ruby>紫陽花<rt>あぢさゐ</rt></ruby>

 <ruby>縦<rt>たて</rt>書<rt>が</rt></ruby>き
 <ruby>紫陽花<rt>あぢさゐ</rt></ruby>

### その他

- 縦書きに特有な表記上の留意点がいくつかある。
    - 日本語には二重引用符""でなくダブルミニュート〝〟を使用した方がよい。
    - 数の表記は「二十三歳」「四、〇〇〇個」「三・一四一六」など漢数字を使用した方が読みやすい場合が多い。
- 縦書きの場合に限らない留意点もついでに。
    - 日本語と英数字との間には半角スペースで間隔を空けるとよい。  
（例：縦書きtumblrテーマ → 縦書き tumblr テーマ）

## 自分用メモ TODO

- **reblog 記事の表示がカオス** (注意：reblog 記事は link 投稿の一種。内容は {Description} 内)
- Edge と IE でタイトルの中央揃えがずれる
- Edge と Windows 版 Chrome でルビのある行間が広くなる
- IE で検索フォームの虫眼鏡が下にずれる
- スマートフォンサイトの作成（iphone-theme.htmlの名で作成予定。<s>横スクロール予定</s>挫折。縦スクロール予定）
- ページ閲覧者によるフォントの切り替え（新字／正字）
- 馬酔木明朝読み込み時のLoading表示

## History

### *2016.02.19*
 - 追加: IE10+, Edge に対応
 - プロジェクトを GitHubGist から GitHub へ移動
 - パノラマのlightbox読み込み時に表示が崩れる問題を修正

さらに以前の更新履歴は [GitHubGistの旧ページ](https://gist.github.com/metasta/5986308)で
