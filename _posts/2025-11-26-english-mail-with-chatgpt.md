---
layout: post
title: 英語をまったく書かずにそれらしい英文メールを作る方法
tags: エッセー コンピューター
---
何やら不思議なタイトルだが、要するに「生成AIは便利である」という話をするための記事である。
友人数名に話すとそれなりに反響があったので、ブログに書くことにした。

### はじめに

所属先を公開しているのでご存じの方も多いかもしれないが、私の職場では、海外の会社と連携して視覚障害者向け支援機器の日本語化と販売をしている。
私が担当する仕事の中に、開発元のエンジニアに不具合報告や機能追加の要望を出したり、技術的な内容についてやり取りをしたりといった作業がある。
ほとんどの場合、連絡手段はメール、使用する言語は英語である。

そんな話をすると、「自分で英語を書いているのか」とか、「英語がものすごく得意なのか」という質問をされることがある。
確かに、英語は決して嫌いではないし、事実、高校時代まで英語を習っていた。
ただ、読むことはともかく、自分で英語を書くのはかなり難しい。
しかも、技術的なややこしい話を英語で書いて、うまく伝わらずに混乱を招くと大変である。

そこで登場するのが生成AIである。
普通の翻訳サービスを使っても良いのだが、ある程度の手直しが必要になるし、「英語のメールとはこういうものだ」という基本的な知識と、多少の経験がないとかなり厳しい。
また、多方面で活用が広がっている生成AIの実力を試してみたいという気持ちもある。

ということで、私が英語のメールを書くときは必ず生成AIを使い、手動での手直しはまったくしない（英語を直接書き換えることはしない）と決めて仕事をしている。
それでどこまで実用的な文章が書けるのか、実際に試しながらご紹介しようと思う。

### 使用するAIサービス

私が使っているのは、OpenAI社のChatGPTである。
他にもいくつかのAIサービスがあり、もっと良いものもあるかもしれないが、「最初に覚えたから」という理由でChatGPTをメインで使っている。

また、私が今回使うのは「Plus」という有料プランだ。
職場では「Team」のプランを使っており、どちらも大きな差はないと思われる。
逆に、無料プランでは多少様子が違うかもしれない。

### 実際にメールを書いてみる

#### 今回取り上げるテーマ

それでは、実際に英語でメールを書いてみよう。
今回は、ソフトウェアのバグ報告を書くことにしよう。

とはいえ、勝手に他者が作ったソフトのバグレポートをでっち上げるわけにも行かない。
そこで、[ACT Laboratory](https://actlab.org/)で私が公開している「[TCV](https://actlab.org/software/TCV/)」に不具合があったと仮定して、それを英語で伝えるメールを書くことにする。

#### 日本語で下書きを作る

まずは、レポートのメイン部分を日本語で作成する。
ここはAIを使わず自分で書けば良いだろう。
誰かが直接読む文章ではないので、意味さえ伝われば、多少書き方が乱暴でも問題はないはずだ。

---

```
TwitCasting Viewer（TCV）で受信したコメントを自動で読み上げる機能について、不具合を見つけました。
実際に受信したコメントと、読み上げられるコメントが1個ずつずれているようです。
たとえば、あるライブに接続した際、古い順にA、B、Cという3つのコメントがコメントリストに表示されたとします。
しばらくして、新たにDというコメントを受信しました。
このとき、音声でもDの内容が読み上げられることを期待しますが、実際には、1つ前のコメントであるCを読み上げてしまいます。
症状の確認と修正をお願いいたします。
```

---

#### ChatGPTに送信して英語の下書きを作る

今作った下書きを、ChatGPTに送って英訳してもらうことにしよう。
「TwitCasting Viewer（TCV）というアプリの不具合報告メールを英語で出したいです。以下の下書きを元に、開発元であるAccessible Tools Laboratoryのサポート窓口に送るメールを作成してください。」というプロンプトに続けて、先ほどの下書きを貼り付けてみる。
すると、こんなメールが作られた（ChatGPTの応答にあった不要な文言を削除したり、メールとしてそのまま送って問題ないように改行などを削除したりという編集を加えている）。

---

```
Subject: Bug Report: Comment Auto-Read Function in TwitCasting Viewer (TCV)

Dear Accessible Tools Laboratory Support Team,

I would like to report an issue I found with the automatic comment reading feature in TwitCasting Viewer (TCV).

It appears that the comment actually spoken by the app is always shifted by one compared to the comment that was just received.
For example, suppose I connect to a live stream and the comment list initially shows three comments in chronological order: A, B, and C.
After some time, a new comment D is received.

In this situation, I would expect the text of comment D to be spoken. However, TCV instead reads out comment C, which is the previous comment.

Could you please investigate and fix this issue?

Thank you very much for your assistance.

Best regards,
Kazuto Kitabatake
```

---

文末に「Kazuto Kitabatake」と書かれている。
これは、おそらくChatGPTのアカウントを登録した際に設定した名前、もしくは過去のやり取りで覚えられた名前ではないかと思う。
ただし、場合によっては名前が入らず、[your name]のように書かれるケースもある。

#### 必要に応じて手直しを依頼する

当初、ChatGPTが提案してきたメールに対して細かな指摘を日本語で出し、修正されていく過程をご紹介しようと考えていた。
しかし、上記のメールは私が想定していた通りの内容になっており、このままACTLabに送っても良さそうだ。
ただ、これでは面白くないので、何か変更させてみよう。

そもそも、ACTLabは日本人の集まりであり、英語ネイティブのメンバーは誰もいない。
ということで、「このメールを受信するのは、英語に堪能でない日本人です。それでも理解しやすいようなメールにしてください。」と頼んでみよう。
現状でも十分理解できるはずだが、どう変化するだろうか。

---

```
Subject: Bug Report: Auto-Read Function in TwitCasting Viewer (TCV)

Dear Accessible Tools Laboratory Support Team,

I found a problem in the automatic comment reading feature of TwitCasting Viewer (TCV).

The comment that TCV reads is shifted by one from the latest received comment.

For example:
- When I connect to a live stream, the comment list shows A, B, and C.
- After that, I receive a new comment D.

In this situation, I expect TCV to read comment D.
But TCV reads comment C instead.

Could you please check this problem and fix it?

Thank you very much.

Best regards,
Kazuto Kitabatake
```

---

先ほどと言っていることは同じだが、表現が極力シンプルなものになった印象がある。

さて、もう少し実験を続けよう。
こうしてChatGPTと共に英語のメールを作りつつ動作を検証していると、最初の下書きの段階では気づかなかった動作を発見することがある。
そのようなとき、場合によっては追加情報として書き添えておくと開発者は助かるかもしれない。
ということで、TCVにもっと複雑なバグが潜んでいたことに気づいたとしよう。
「さらにテストを続けたところ、ライブに接続した時点の状況によって動きが変わることがわかりました。オフライン状態（ライブ開始前）に接続し、ライブの開始、新しいライブでの最初のコメントをリアルタイムに受信した場合は、受信したコメントを正しく読み上げます。しかし、すでに始まっているライブに接続した場合は、先ほどの下書きに書いた状況になります。このテスト結果も反映させて、再度メールを作ってください。」

---

```
Subject: Bug Report: Auto-Read Function in TwitCasting Viewer (TCV)

Dear Accessible Tools Laboratory Support Team,

I found a problem with the automatic comment reading feature in TwitCasting Viewer (TCV).
I would like to share the details and my test results.

1. Main problem

TCV sometimes reads the wrong comment.
The spoken comment is one comment older than the newest received comment.

Example:
- The comment list shows A, B, C when I connect.
- Later, a new comment D arrives.
- I expect TCV to read D, but TCV reads C.

2. Additional test results

The behavior changes depending on the timing of the connection:

Case 1: Connect before the live starts (offline state)
- When the live starts and the first comment is received in real time, TCV reads the correct comment.
- This behavior is normal.

Case 2: Connect after the live has already started
- When joining an ongoing live, TCV shows older comments first and then receives a new comment.
- In this case, TCV reads the previous comment instead of the new one (the problem described above).
- This happens every time in my tests.

Could you please check this issue and fix it?

Thank you very much for your support.

Best regards,
Kazuto Kitabatake
```

---

かなり複雑な現象だが、このメールならばおそらく問題なく伝わるだろうと思う。
実際に、私がもしこのメールを受け取ったとしても、何が起きているかは大体想像できるはずだ。
ちなみに、実際のTCVにはこんな不具合はないのでご安心いただきたい。

### 返信メールへの対応について

一人二役でメールを書くのは大変なので、今回は取り上げないが、相手から返信が来たらどうするかということにも触れておいた方が良いだろう。
私の場合は、まず届いた英語のメールをそのまま読んでみる。
その結果によって、自然と次のアクションが決まる。

英語のままで概ね内容がわかり、返信したい内容が頭の中にあれば、すぐ返信メールの作成に取りかかれる。
「以下の返信が来ました。こういう内容で返事を出したいです。」とChatGPTに伝えれば良い。

逆に、英語を読んでも意味がわからなければ、「以下の返信が来ました。内容を日本語にしてください。」と頼んでみる。
その回答を読んだ上で改めて英語を見ると、最初よりは意味が理解しやすくなる。
そうなれば、後は返信を考えるだけだ。

### 最後に

こんなことを書いていると、「AIに書かせるなんてインチキだ。きちんと自分でメールを書かないといけない」というお叱りが聞こえてきそうな気がする。
確かにそういう感覚は私にもはある。

しかし、今回取り上げたようなメールを送る目的は、ソフトウェアをより良くすることであり、スムーズにコミュニケーションを取れた方が良いはずだ。
そのための道具として生成AIを使うのは、決して悪いことではないと最近感じている。

実際のところ、上記のような方法でメールを書いたとしても、読み手はAIで書いたということにほとんど気づかないようだ。
先日、普段仕事で頻繁にやり取りをしている会社の担当者が、「最近メールを送ってくるようになったKazutoさんという人は、かなり英語ができる人なんですね」と言っていたと、私の上司から聞いた。

その一方、日本語の文章を書くツールとしては、ChatGPTをほとんど使わない。
その理由は、自分の中に自然と作られてきた「私らしい文章」を書くことが、AIにはできないからだ。
とはいえ、もう少しすればこの問題は解決するだろう。
私が書いたメールを学習させておけば、私らしい文章を書いてくれるかもしれない。

引き続きAIの進化を見守りながら、使えそうなものはどんどん使っていきたいと思っている。
