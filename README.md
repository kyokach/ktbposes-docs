# KTBPoses マニュアル

VRChat アバター向けのポーズ集ツール **KTBPoses** のマニュアルです。

https://kyokach.github.io/ktbposes-docs/

このリポジトリにはマニュアルだけが入っています。ツールのソースコードと .unitypackage は含みません。

## 手元で見る

```
pip install -r requirements.txt
mkdocs serve
```

## 公開

`main` に push すると、GitHub Actions（`.github/workflows/docs.yml`）が MkDocs で組み立てて GitHub Pages に公開します。
プルリクエストでは、組み立てられるかどうか（`mkdocs build --strict`）だけを確かめます。
