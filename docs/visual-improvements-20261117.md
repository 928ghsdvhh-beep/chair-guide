# 画像・記事入口の改善（2026年11月17日）

チェア：既存の白と深緑のデザインを継承し、写真左・記事案内右の小さな導入を追加。設置・搬入・調整の3記事に直接進める。写真幅は通常210px、スマホ96px、設置記事内は最大360px/スマホ280px。

## 画像

built-in imagegenで生成した900×600pxのWebP。AI生成のイメージと明示し、掲載商品の実写真や実測の根拠として扱わない。元生成は1536×1024px。無断の商品写真転用なし。

生成プロンプト：photorealistic natural tidy Japanese home workspace, unbranded black mesh office chair beside light oak desk, clear visible space, soft daylight, no people/logos/text, generic lifestyle setting, not a branded product model.

## 検証

静的監査 issues 0。内部リンク・canonical・sitemap・JSON-LDを検証。全既存公開HTMLのA8アンカー・計測画像とCloudflare解析scriptを変更前と完全照合し一致。git diff --check成功。画像寸法属性で表示領域を確保。広告素材の寸法・コードは維持。公開版とブラウザの狭幅確認は別途実施。
