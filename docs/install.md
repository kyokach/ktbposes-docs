# インストール

## 必要なもの { #requirements }

| | バージョン |
|---|---|
| Unity | 2022.3（VRChat が指定するバージョン） |
| VRChat SDK - Avatars | 3.5.0 以上 |
| Modular Avatar | 1.18.0 以上（NDMF は Modular Avatar と一緒に入ります） |

Unity 2022.3.22f1、VRChat SDK - Avatars 3.10.4、Modular Avatar 1.18.1 で動作を確かめています。ポーズを入れるアバターは Humanoid である必要があります。

## 入れかた

1. VCC（VRChat Creator Companion）などで、プロジェクトに Modular Avatar を追加します
2. Unity のプロジェクトを開き、`KTBPoses_v<バージョン>.unitypackage` をプロジェクトのウィンドウにドラッグ＆ドロップします
3. すべてにチェックが入った状態で「Import」を押します
4. メニューの **Tools → KyokaToyBox → KTBPoses** で開きます

`Assets/KyokaToyBox/KTBPoses` に入ります。

### 最初に開いたとき

アニメーションライブラリ（同梱の 100 ポーズ入り）と、それを 6 つのサブメニューに分けたポーズ集「KTBPoses」を作ります。そのまま [アバターに導入](quickstart.md) できます。

| フォルダ | 中身 |
|---|---|
| `Assets/KyokaToyBox/KTBPoses` | ツール本体と、同梱ポーズのアニメーション |
| `Assets/KyokaToyBox/KTBPosesData` | このプロジェクトのアニメーションライブラリとポーズ集 |
| `Assets/KyokaToyBox/Generated/KTBPoses` | アバターに導入するときに作るもの（アバターごと） |

!!! note "Modular Avatar が入っていない・古いとき"
    **Tools → KyokaToyBox → KTBPoses** を開くと、必要なパッケージと、プロジェクトに入っているバージョンを表示します。エラーにはなりません。VCC で Modular Avatar を追加・更新すると、ツールが使えるようになります。

## 更新するとき { #update }

!!! warning "先に `KTBPoses` フォルダを消してください"
    .unitypackage は、新しい版で無くなったファイルを消しません。古いファイルが残ると、正しく動かないことがあります。Unity で `Assets/KyokaToyBox/KTBPoses` を消してから、新しい .unitypackage を入れてください。

`KTBPosesData`（ライブラリとポーズ集）と `Generated/KTBPoses`（導入で作ったもの）は消さないでください。どちらも .unitypackage には含まれないので、更新しても上書きされません。

更新したら、導入済みのアバターで [導入し直す](install-avatar.md#reinstall) を押してください。アニメーターとメニューが新しい版になります。[同梱ポーズを体型に合わせ直して](library.md#refit) いた場合は、もう一度合わせ直してください（同梱ポーズのアニメーションが元に戻るため）。

### 新しく増えた同梱ポーズ

新しい版で増えた同梱ポーズは、更新したあと最初にツールを開いたときに、ライブラリへ追加されます（カテゴリのタグ付き）。2.0 から 2.1 に更新すると、74 ポーズが増えます。

- 今あるポーズ集は変わりません。増えたポーズを入れるときは、[ポーズ集](pose-sets.md) タブで追加するか、**同梱から作成** で全ポーズのポーズ集を作ってください
- ライブラリから外していた同梱ポーズは、更新しても戻りません

## アンインストール { #uninstall }

1. 導入したアバターごとに、[取り外す](install-avatar.md#uninstall) を押します
2. `Assets/KyokaToyBox/KTBPoses`、`Assets/KyokaToyBox/KTBPosesData`、`Assets/KyokaToyBox/Generated/KTBPoses` を消します
