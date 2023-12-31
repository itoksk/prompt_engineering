
# Lesson 1: プロンプトエンジニアリングとオブジェクト指向の基礎 (20分)

## 良いプロンプトの構造と明確な指示の出し方、そしてそのオブジェクト指向的な見方の説明

曖昧な指示：「教えて」

明確な指示：「第二次世界大戦中のアメリカの経済状況について、3つの主要なポイントで説明してください」

これらのポイントに従って明確な指示を与えることで、GPTモデルから正確で質の高い回答を得ることができます。


## プロンプトエンジニアリングの基礎

GPTモデルに明確な指示を与えることは、正確で意図通りの回答を得るために非常に重要です。以下に、モデルへの明確な指示を書く際のいくつかのポイントを示します。

良いプロンプトは、以下の要素を含むことが望ましいです。

### 1. 明確な指示
- [ ]  タスクが何であるかをはっきり記述し、それに関連する背景情報を提供して、GPTに期待する応答を明示します。
- [ ] 質問または指示は短くても意味が伝わるように簡潔に記述します。
- [ ] 冗長なフレーズは避け、モデルが理解しやすい言葉を使用します。

|悪い|良い|
|-|-|
|野球の特徴|初心者が野球を楽しんで観戦するために知っておくべき主要な特徴|

### 2. 引き締めた文脈
- [ ] 必要な情報や制約条件を適切に与え、回答の枠組みを明確にする。

|悪い|良い|
|-|-|
|Pythonでリストをソートする方法|Pythonで数値が格納されたリストを降順にソートする方法|

### 3. 丁寧なフィードバック
- [ ] ChatGPT の応答を評価し、次のプロンプトに活用して、性能を向上させる。

### 4. 文脈設定
フォーマットを指定します。プロンプトに適切な背後情報や制約を提供して、応答の精度を向上させます。あなたがどのような形式で回答を受け取りたいかを伝えることで、回答が理解しやすい形で提供されるようになります。

|悪い|良い|
|-|-|
|ネットワークの基本|ニューラルネットワークの基本的な概念を3つの要点で簡潔に説明してください|

### 5. ペルソナ設定
 - [ ] モデルにペルソナ（例：親切な助言者、専門家、コメディアン）を学習させるように付け加えることで、さらにユニークで創造的な回答を得られるようになります。
 - [ ] ペルソナのスタイルやトーンに沿った回答を得るために、その指定を明確に伝えます。例えば、親しみやすいトーンや古風な表現、専門的な言葉を使うようにリクエストできます。
 - [ ] ペルソナの専門知識や経験に関連する質問をすることで、モデルはその知識を最大限に活用し、ペルソナに合った回答を提供します。
 
|-|良い|
|-|-|
|1|アインシュタインとして、相対性理論を簡単に説明してください。|
|2|シェイクスピア風の文体で、自然保護の重要性を語ってください。|
|3|古代ローマの歴史家として、カエサルの業績について語ってください。|

ペルソナ採用の指示を明確にし、適切なスタイルやトーンを要求することで、モデルはそのペルソナに沿った情報や視点をもとに、独自性のある回答を提供します。

オブジェクト指向的な見方では、プロンプトはオブジェクト（データと機能の集合）として扱われ、プロンプトに対する期待や制約はオブジェクトの状態・振る舞いとなります。

この視点でプロンプトを設計することで、再利用性やモジュール性が向上し、メンテナンスも容易になります。

## デモンストレーション

例：「あなたは格闘アニメが好きな高校生です。お気に入りの漫画の登場人物の中で、最も好きなキャラクターを選び、そのキャラクターが魅力的だと思う理由について、100文字以内で3つ述べてください。」

また、指示は明確で、「最も好きなキャラクター」を選び、その理由を「3つ」述べることが求められています。

プロンプトで明確に指示を与えているため、回答者はどの漫画の登場人物を対象に選んだかがわかります。

また、ここでのプロンプトは、
```
1. ペルソナ（格闘アニメが好きな高校生）
2. 登場人物（お気に入りの漫画)
3. レベル（最も好き）
4. 温度（魅力的な理由）
5. 制限（100文字以内、3つ）
```
上記の構成要素を持つ


## アクティビティ

1. 「理想の高校生活について述べてください」というプロンプトを、期待した応答を生み出すシンプルなプロンプトを作成しよう。  
   `出力させたい結果をイメージして、そのイメージ通りの結果が出るように、プロンプトを考えよう。`

3. そのプロンプトを構成している要素について解釈を考えよう。

        - 精緻化されたプロンプト:

        - 高校生活は、どのような構成要素を持つ?
        　 　1. 
        　 　2.
          3.  
          4.  
          5.  

このような、解釈を考えることで、他の領域（例：理想の大学生活、理想の仕事環境）でもプロンプトが適用可能であることがわかります。
