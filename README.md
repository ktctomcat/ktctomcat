## Hi there 👋

<!--
**ktctomcat/ktctomcat** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->

![TomooDesign Works](https://ktctomcat.github.io/assets/img/ogp.png)

GitHub Pages を用いて、地域情報等を発信する Web サイトの作成を試みています。

I am trying to create a website using GitHub Pages to provide local information.

### Come on!

![かもん！カモねぎくん](https://ktctomcat.github.io/assets/img/kamonegi-kun_classic_logo.png)

[かもん！カモねぎくん](https://ktctomcat.github.io/kamonegi/)

このサイトでは「かもん！カモねぎまつり」の情報やキャラクターの「カモねぎくん」に関連する画像データ等を公開しています。  
是非訪れてみてください。

This site provides information about the "Come on! Kamonegi Festival," held every year on the first Sunday of December in the Katahigashi area of Nishikan Ward, Niigata City, Niigata Prefecture, Japan. It also features images of the mascot "Kamonegi-kun."  
We invite you to visit us!

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=ktctomcat&layout=compact)](https://github.com/anuraghazra/github-readme-stats)




表示されない原因のよくあるパターンと直し方

- 記法のミス: 送ってくれた行は、画像をリンクでラップする書き方が途中で崩れてます。正しくは「画像の前にもう一つ [」が必要です。  
  下の修正版をそのまま貼ってみてください。

`markdown
![Top Langs](https://github.com/anuraghazra/github-readme-stats)
`

- サービス側の一時的エラー: GitHub Readme StatsはVercel上で動いていて、負荷やレート制限で「Maximum retries exceeded」などのエラーで画像が返らないことがあります。自分のVercelにフォークしてホスティングし、PAT_1 環境変数にGitHubのトークンを設定すると安定します。

---

動作確認のチェックリスト

- URLを直接開く: ブラウザで画像URLだけを開いて、画像が出るか確認。  
  例: https://github-readme-stats.vercel.app/api/top-langs/?username=ktctomcat&layout=compact  
  エラーメッセージが出るなら、サービス側の問題の可能性が高いです。

- キャッシュの待ち/指定: 一時的な失敗でも時間を置くと復帰することがあります。明示的に  
  &cacheseconds=7200 などを付けてキャッシュを長めにすると負荷を減らせます。

- Vercelセルフホスト: フォーク→自分のVercelでデプロイ→PAT_1 を設定→URLを自分のデプロイに差し替え。  
  これでレート制限の影響を受けにくくなります。

---

そのまま使える差し替え例

- 最小修正（記法のみ修正）
`markdown
![Top Langs](https://github.com/anuraghazra/github-readme-stats)
`

- キャッシュとテーマを追加
`markdown
![Top Langs](https://github.com/anuraghazra/github-readme-stats)
`

- セルフホストURLに差し替え（例）
`markdown
![Top Langs](https://github.com/anuraghazra/github-readme-stats)
`
> セルフホストは、負荷分散とレート制限回避に有効です。

---

うまくいかなかったら教えてほしいこと

- READMEの場所: プロフィール用のリポジトリ（ktctomcat/ktctomcat）のルートに README.md があるか。  
- 現在の表示: 何も出ないのか、エラーテキストが画像枠に出ているのか。  
- URL直開きの結果: 画像が表示されるか、エラーメッセージか。

一緒に最短で直します。直近は記法の修正がいちばん効きます。その次にURL直開きの確認、必要ならセルフホストに切り替えましょう。


