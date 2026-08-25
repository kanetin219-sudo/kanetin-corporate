# 株式会社かねちん コーポレートサイト

## 公開のしかた（5分）

### Netlify Drop ＝ 一番早い。アカウント不要
1. このzipを解凍する
2. https://app.netlify.com/drop をブラウザで開く
3. 解凍してできたフォルダを、画面にドラッグ＆ドロップ
4. URLが表示される（例：https://xxxx.netlify.app）

### GitHub Pages ＝ 無料・商用OK・独自ドメイン可
1. GitHubで新しいリポジトリを作る（Public）
2. 解凍したフォルダの中身を全部アップロード
3. Settings → Pages → Branch を main にして Save

### Vercel
Hobbyプランは商用利用不可のため、会社サイトに使うならProプラン（月20ドル）が必要です。

---

## ファイル構成
```
index.html        トップページ
jisseki.html      実績
b-gata.html       就労継続支援B型（アネラカフェ大分）
privacy.html      プライバシーポリシー
tokushoho.html    特定商取引法に基づく表記
style.css         共通スタイル
favicon.png       ファビコン
img/              写真20枚
```
`preview/` は確認用です。アップロード不要。

---

## 公開前に必ず埋めるもの

### 法令上、空欄のままにできないもの
- [ ] tokushoho.html の全項目（Lゼロで受講料を受け取っているため法律上必須）
- [ ] privacy.html の連絡先・アクセス解析の項目
- [ ] 就労継続支援B型 事業所番号（b-gata.html／index.html）
- [ ] 第一種動物取扱業 登録番号・登録年月日・有効期間・動物取扱責任者（b-gata.html）

### これがないと問い合わせが来ない
- [ ] 所在地、電話番号
- [ ] 問い合わせフォームのURL（index.html の「お問い合わせフォームへ」）
- [ ] 工賃（b-gata.html／ご家族が最も見る項目）
- [ ] 対象となる方、定員、送迎、食事（b-gata.html）

### 画像・文章
- [ ] logo.svg（濃色）/ logo-white.svg（白）※いまは社名テキストで表示中
- [ ] img/daihyo.jpg（代表写真・縦位置）
- [ ] 代表挨拶の本文（下書きが入っています）
- [ ] 沿革の年月3つ（独立／Lゼロ開講／アネラカフェ開設）
- [ ] おでかけ隊のURL
- [ ] 保護犬猫カフェのテレビ出演：番組名と放送日
- [ ] アカウントのアイコン画像4枚（いまは頭文字で表示中）

### 掲載同意の確認
- [ ] 店内写真に写っているお客様
- [ ] 実績ページに載せた支援先の投稿画面

---

## 差し替え方のメモ

**写真を入れ替える**
img/ の中の同名ファイルを上書きするだけ。HTMLは触らなくて大丈夫です。

**アカウントのアイコンを入れる**
img/ に `sns_kanetin.jpg` などを置き、index.html の該当箇所のコメント行と
`<span class="account__ava">か</span>` を入れ替えてください。

**ロゴを入れる**
logo.svg と logo-white.svg を置き、各HTMLヘッダーのコメントを外して
`<span class="hdr__logotext">` の行を削除してください。
