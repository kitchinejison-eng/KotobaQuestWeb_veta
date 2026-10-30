# KotobaQuest V84 UI refinement — mobile / smartphone / tablet

## 変更内容

- 構音筋ビジュアルナビゲーションを再構成。解剖図と注目部位・説明・ステップを同じカードに整理し、下段にお手本再生・マイク・認識結果を配置。
- スマートフォン縦向きでは上下2段、横向きおよびタブレットでは左右2カラムに切り替える。
- 図のハイライト、マイク認識状態、既存の音声練習イベントIDと判定処理を維持。
- ことばクエストZを再構成。HUD、敵・勇者、問題文、判定、選択肢を画面内に配置。
- スマートフォン縦向きでは縦のバトルボード、横向きおよびタブレットでは戦況と回答を左右に配置。
- 選択肢は番号付きの見た目にし、ボタンのtextContentと既存の正誤判定ロジックは変更しない。
- ホームのジャンルカードをスマートフォン2列、タブレット縦3列、広いタブレット横4列に最適化。
- Androidのアプリ名は「ことクエ」、applicationIdは `jp.co.aristoteles.kotobaquest.prototype` を維持。画面回転は `unspecified` のまま縦横に対応。

## Android version

- versionCode: 7
- versionName: 0.7.0
- applicationId: jp.co.aristoteles.kotobaquest.prototype

既存の試作アプリを更新する場合は同じ署名鍵でビルドしてください。本番アプリとは別IDのままです。

## 確認

- Web / Android WebView asset JavaScript files: `node --check` passed.
- CSS files: syntax parsed without errors.
- HTML IDs: no duplicate IDs found.
- Local HTML asset references: no missing references found.
- ZIP integrity: verified with `unzip -t`.
- Android Gradle APK build: not completed in this environment because Gradle 9.6.0 could not be downloaded from services.gradle.org (network unavailable). Build with Android Studio or an internet-connected Gradle environment.

## 展開場所

Windowsでは日本語を含まないフォルダに展開してください。例：`C:\AndroidProjects\KotobaQuest\`
