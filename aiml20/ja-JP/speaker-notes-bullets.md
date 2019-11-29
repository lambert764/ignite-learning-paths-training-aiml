# <a name="aiml20-speaker-notes"></a>AIML20:講演者用メモ

スクリプト化されたテキストではなく箇条書きから作業する場合は、PPT プレゼンテーションの各スライドの主要なポイントを次に示します: https://microsoft.sharepoint.com/:p:/t/CloudDevAdvocacy/EctuTXQCOdpGqc5lhQgUnMgBr-R6hlWR5MuLE3qCIFgoHA?e=r1szwF

関連するデモ スクリプトについては、 https://github.com/microsoft/ignite-learning-paths/tree/master/aiml/aiml20 を参照してください。 `DEMO%20Setup.md`で開始します。

## <a name="slide-notes"></a>スライド メモ

スライドはタイトルでのみ識別されます。

### <a name="slide-microsoft-ignite-the-tour"></a>スライド:Microsoft Ignite the Tour

プレゼンテーション前の導入スライド

### <a name="slide-using-pre-built-ai-to-solve-business-problems"></a>スライド:事前構築済み AI を使用してビジネスの課題を解決する

自己紹介します。

コンピューティング リソースや AI の専門知識がない場合でも、AI 機能をアプリケーションに追加する方法。

クラウドで事前構築された AI サービスを使用する。

### <a name="slide-resources"></a>スライド:リソース

豊富なリンク、リソース、デモを用意しています。

完全なソース コードとアプリのワンクリック デプロイを含むすべてのリンクについては、こちらのリンクを参照してください。

このスライドは、最後に再び表示されます。

### <a name="slide-adding-humanlike-capabilities-to-apps"></a>スライド:人間的機能をアプリに追加

事前構築された AI サービスを使用してアプリケーションに人間的機能を追加します。それはどのような意味があるのでしょうか。 次に例をいくつか示します。

### <a name="slide-enhance-apps-with-humanlike-capabilities"></a>スライド:人間的機能を使用してアプリを強化する

[クリック] アプリに音声の機能 (チャットなど) を追加します。
 
[クリック] アプリに表示させる機能を追加します (イメージを理解する)。

[クリック] アプリに人間の行動に関する直感を与えます (インターフェイスを適応させる)。

[クリック] アプリに読解力を与えます (あらゆる言語でコミュニケーションする)

[クリック] 異常 (およびスケーリング) のデータ ストリームをスキャンする人によるプロセスを自動化する

いくつかの例を示します。

### <a name="slide-overview-of-azure-cognitive-services"></a>スライド:Azure Cognitive Services の概要

人間的 AI を実装するには、大量のデータと技術的な専門知識が必要ではありませんか。

答えは、いいえです。 Microsoft Research の専門知識を活用してください。 単純な REST API 呼び出しを使用して機能を追加します。 

これが、Azure Cognitive Services です。

### <a name="slide-azure-cognitive-services"></a>スライド:Azure Cognitive Services

Azure Cognitive Services には、20 を超える数の API が用意されています。

人間的能力のカテゴリに含まれるサービス:

視覚:写真、描画、テキストと手書き、ビデオ内容の認識

音声:音声を理解して認識し、自然な人間的な音声を生成するツール。

言語:文書やテキストの内容を解釈し、人間の言語間で翻訳します。

デシジョン: Azure Cognitive Services の最新のカテゴリで、データ、コンテンツ、アプリケーション ユーザー インターフェイスについて人間のような選択を行うことを目的としています。

検索: 大規模な非構造化リポジトリのコンテンツに関する自然言語の質問に回答します。 

### <a name="slide-azure-cognitive-services-with-service-names"></a>スライド:Azure Cognitive Services (サービス名を含む)

"Search" は既に説明されています。 

他の利用可能なサービスを使用して、小売用 Web サイトを強化します。 [クリック]

Computer Vision: 製品の写真のコンテンツを分析するために使用します。

Custom Vision: 小売業者が販売する製品を特定するために使用します。

Personalizer: Web サイトのレイアウトを自動的に適用します。 

ただし、Cognitive Services の設定と使用の原則はすべての API で同じであり、ここで学習する内容は、これから使用したい AI サービスにも適用されます。

### <a name="slide-computer-vision"></a>スライド:Computer Vision

まず、Computer Vision 用に事前構築された AI を見てみましょう。

### <a name="slide-shop-by-photo"></a>スライド:Shop By Photo

これは、Tailwind Traders、ハードウェアの小売販売業者 (架空の会社) の Web サイトです。 

### <a name="slide-demo-shop-by-photo"></a>スライド:デモ:Shop by Photo

デモ:"問題の定義:Shop by Photo が壊れています"

### <a name="video-shop-by-photo"></a>ビデオ:Shop by Photo

Tailwind Traders のライブ Web サイトにアクセスしてみましょう。 [クリック]

AI 対応の機能の 1 つに、"Shop by Photo" (写真でショッピング) と呼ばれるものがあります。 この機能を使用すると、顧客は購入する可能性のある製品の写真をアップロードできます。また、製品が購入可能かどうかをアプリで通知を受け取ることができます。 さあ、試してみましょう。 まず、興味のあるドリルの写真をアップロードします。Tailwind Traders アプリは画像を分析し、それがドリルであることを認識して、Tailwind Traders が販売しているドリルとサイト内のどこにあるかを示します。

では、別の画像で試してみましょう。 ホームページに戻り、"Shop by Photo" 機能をもう一度使用してみましょう。今回は、一組のプライヤーの画像を選びます。 残念ながら、アプリがその画像を分析すると、ハンマーであると認識します。 これは明らかにうまく機能していないので、今度は何が悪かったのかを見つけ、Computer Vision を使用して、修正する方法を見てみましょう。 

### <a name="slide-how-computer-vision-works"></a>スライド:Computer Vision のしくみ

ここでは、少し理論的に説明します。 数学的ではありません。

問題の原因と解決方法を理解するのに役立ちます。

### <a name="slide-tasks-xkcd-comic"></a>スライド:タスク (XKCD コミック)

(10 秒間一時停止)

写真を理解するコンピューターというのは、かつては文字通りサイエンス フィクションにすぎませんでした。

5 年後、これは不可能なことではなく、簡単にできるでしょう。

### <a name="slide-how-neural-networks-work-brandon-rohrer"></a>スライド:ニューラル ネットワークの仕組み (Brandon Rohrer)

Brandon Rohrer から許可を得て改変しています。

ビデオ チュートリアル シリーズのブログをご覧ください。AI と機械学習に関する多くの特徴について詳しく説明しています。 

### <a name="slide-computer-vision--convolutional-neural-network"></a>スライド:Computer Vision / 畳み込みニューラル ネットワーク

AI は "ディープ ラーニング" によって機能しますが、"ディープ" は " 深い" を意味するものではありません。

これは単純な NN （ニュートラル ネットワーク）です。 実際には多くのレイヤーがあります。

5 つのオブジェクトだけを検出するように設計されています。 それ以外のものを認識することはできません。

### <a name="slide-trained-convolutional-nn"></a>スライド:トレーニング済み畳み込み NN

入力画像が左側に移動します。 

各ノードは、元の画像を処理して再結合し、分類の信頼度が最後に単一の値になるまで圧縮します。

ここでは、入力が自転車で、右側のノードの値が "bicycle" になっています。 画像が正しく識別されました。

### <a name="slide-filters-1"></a>スライド:フィルター (1)

時間をあけます。

### <a name="slide-filters-2"></a>スライド:フィルター (2)

時間をあけます。

### <a name="slide-filters-3"></a>スライド:フィルター (3)

時間をあけます。

### <a name="slide-training-an-image-classifier"></a>スライド:画像分類のトレーニング

では、これを行うために NN をどのようにトレーニングすればよいでしょうか。

[クリック] 右側のフィルターを選択します。 各フィルターは、重みの小さいグリッド (通常は 3 x 3 または 5 x 5) によって制御されます。

[クリック] 分類がわかっている多くのトレーニング イメージを使用して重みを選択します。 正しい分類が選択 (または、少なくとも多くの場合) されるように、重みを選択します。

実際のビジョン ネットワークでは、数百万の重みを選択できます。 重みはどのように決定されますか。

### <a name="slide-learning-backpropagation"></a>スライド:学習:誤差逆伝搬法

ここでは、かなりの数値演算が登場します。

ですが、AI エンジニアにでもならない限り、気にする必要はありません。 重みが他のユーザーによって最適化されたネットワークのみを使用できます。

これは、アプリケーションの約 80% をカバーしています。 ただし、独自の NN を設計して重みを最適化する必要がある場合は、Tensorflow や PyTorch のようなツールがあります。 AIML40 と AIML50 の内容について説明します。

### <a name="slide-pre-trained-convolutional-nn"></a>スライド:事前にトレーニング済みの畳み込み NN

しかし、必要な画像を検出できる NN にアクセスできる限り、画像を提供するだけで十分です。ネットワークがユーザーのために分類します。

モデルによっては、単に分類するだけでなく、オブジェクトの場所を検出したり、他の方法で画像を分析したりすることができます。

### <a name="slide-demo-cognitive-services-computer-vision"></a>スライド:デモ:Cognitive Services Computer Vision

Cognitive Services Computer Vision には、数千ものオブジェクトを分類できる強力な NN が用意されています。

aka.ms/try-computervision にあるシンプルな Web ベースの UI を試用できます

今すぐ試してみましょう。

### <a name="video-computer-vision-via-web"></a>ビデオ:Web を使用した Computer Vision

[クリック] これは Cognitive Services Computer Vision のページです。 このページで、少し下にスクロールすると、Web ベースのフォームがあります。Ｗeb から、またはローカル ファイルとして、分析用の画像をアップロードできるようになります。 では、ヘルメットを被っている男性の写真をアップロードしてみましょう。 ほんの数秒で、Computer Vision サービスからその画像の分析が返されます。 左側には、画像内の検出されたオブジェクト、右側には、詳細な分析を含む JSON 形式の出力が表示されます。 これには、画像内の検出されたオブジェクトの名前と場所、画像に関連付けられているタグまたはラベルの一覧、画像についての平易な説明 (この場合は "ヘルメットを被っている男性")、およびその他の有用な情報が含まれます。

### <a name="slide-cognitive-services-computer-vision"></a>スライド:Cognitive Services Computer Vision

オブジェクトの検索: 2 つのオブジェクトが検出されました。 頭に装着するもの、人。

タグを確認します。 最高の信頼性: 人。 次は頭に装着する物です。 ヘルメットは 6 番目です。
"ヘルメット" のモデルは特にトレーニングされていません。

この問題を解決する方法について、すぐに説明します。

アプリにビジョンを組み込む場合は、プログラムを使用して API にアクセスできます。 その方法を見てみましょう。

### <a name="video-computer-vision-via-cli"></a>ビデオ:CLI を使用した Computer Vision

HTTP エンドポイントに接続できる任意の言語を使用して、Cognitive Service API にインターフェイスを設定することができますが、ここでは、[クリック] Azure CLI を使用してリソースを作成し、"curl" を使用して Computer Vision API に接続する bash スクリプトを使用します。 ローカル シェルに Azure CLI をインストールできますが、ここでは Visual Studio Code の "Azure アカウント" 拡張機能を使用して Cloud Shell を起動します。つまり、何もインストールする必要はありません。 シェルの準備ができたら、この bash スクリプトから直接コマンドを実行できます。 

最初のコマンドで、リソース グループを作成します。これは、API を認証するために必要なキーを保持するために使用します。

次の手順で、キーを作成します。 ここでは、Computer Vision を含む多くのサービスで使用できるオムニバスの Cognitive Services キーを作成しています。

これで、キーをターミナルに直接表示できます。 [待機] これらのキーのいずれかを使用して API とやり取りすることができるので、最初のキーを環境変数に保存します。

このキーを使用すると、Computer Vision サービスによって提供されるエンドポイント URL に接続できるため、その URL を環境変数に保存することもできます。

次に、分析する画像を選択できます。 ここでは、イメージの URL を指定します。これは、少し前に見たヘルメットを被る男性と同じイメージです。

ここで、curl を使用して JSON 入力を渡すことによって、キーとイメージ URL をエンドポイントに渡すことができます。 数ミリ秒で、JSON としてイメージ分析が返されます。 前に Web インターフェイスで見たものと同じ出力が表示されます。

もちろん、好きなイメージを使って行うことができます。 別の画像 (この場合はドリルの画像) でもう一度試してみましょう。 ここでも、curl を使用して API に渡すことができます。 [待機] 興味深いことに、このイメージに関連付けられている最上位のタグは "カメラ" で、残念ながら実際の工具を検索するのには役立ちません。"ドリル" が必要です。

### <a name="slide-adapting-computer-vision-models-with-your-own-data"></a>スライド:Computer Vision モデルを自身のデータに適合させる

Computer Vision API は、Shop by Photo では機能しません。 

あまりに多くのオブジェクトの種類を検出するようにトレーニングされています。

幸い、この問題を解決することができます。 では、少し理論について説明しましょう。

モデルを何千ものオブジェクトに適合させ、目的のオブジェクトだけを検出するように調整する方法があります。 たとえ元のモデルに含まれていなかった場合でも。 

Transfer Learning と呼ばれる AI 手法を使用して、その方法を見てみましょう。 

### <a name="slide-transfer-learning"></a>スライド:Transfer Learning

最後のレイヤーがオフになっている場合と同じ CNN。

2 番目の最後のレイヤーは "特徴" を提供します。これは数値のベクターと考えることができます。 各イメージは、異なる特徴のセットを生成します。

特徴が何を表わすのかわかりませんが、一般的にはイメージを分類するのに役立ちます。

トリック: これらの特徴を使用して、オブジェクトの新しいセットを分類できます。

### <a name="slide-transfer-learning-training-1---with-the-hammer"></a>スライド:Transfer Learning のトレーニング (1 - ハンマー)

Transfer Learning を使用して、ハンマーとヘルメットを識別するモデルを作成します。

ハンマーの写真を渡し、特徴を収集します。 さらに "ハンマー" のバイナリ インジケーターを収集します。 多くのハンマーに対して繰り返します。

### <a name="slide-transfer-learning-training-2---with-the-white-hard-hat"></a>スライド:Transfer Learning のトレーニング (2 - 白いヘルメット)

ここで、ヘルメットの画像を使用して同じ操作を行います。

いずれの場合も、8 つのデータ ベクターと各イメージのバイナリ インジケーターを収集します。

すべてをまとめて、それぞれにバイナリの結果が関連付けられたデータ ベクターのコレクションを作成します。 

これにより、簡単な予測モデルを作成できます。

### <a name="slide-transfer-learning-trained-model"></a>スライド:Transfer Learning トレーニング済みモデル

これは驚くほどうまく機能します。

大量の画像や演算能力は必要ありません。

これはおもちゃの例ですが、この原則は大規模なモデルにも当てはまります。

### <a name="slide-microsoft-cognitive-services-custom-vision"></a>スライド:Microsoft Cognitive Services Custom Vision

Transfer Learning モデルを自分でトレーニングする必要はありません。

Microsoft のトレーニング済みのビジョンモデルの 1 つを使用して、Custom Vision で独自のオブジェクトのイメージを適応させます。

Shop by Photo 用のビジョン モデルを作成してみましょう。

### <a name="slide-demo-customized-object-recognition"></a>スライド:デモ:カスタマイズされたオブジェクトの認識

デモの手順: https://github.com/microsoft/ignite-learning-paths/blob/master/aiml/aiml20/DEMO%20Custom%20Vision.md

### <a name="video-customvisionai"></a>ビデオ: customvision.ai

[クリック] ここで、Custom Vision Web ベースのインターフェイスについて説明します。 転移学習分析用に新しい画像を提供するのに優れた UI が提供されています。 このプロジェクトには、既に多数の画像がアップロードされています。 ドライバー、ペンチ、ドリル、ハンマーの写真をアップロードしました。これは、カスタムモデルのトレーニング用に使用します。 また、Tailwind Traders が販売しているもう 1 つの製品 (ヘルメット) を検出することもできます。 ここで、[イメージの追加] をクリックし、ハードドライブ上のフォルダーを参照して、ヘルメットの写真をいくつか収集し、それらをすべて選択してサービスに追加し、トレーニングで使用する "hard hat" というラベルを指定します。

これらのファイルをアップロードするには、しばらく時間がかかります。その間は、このプロジェクトに多くの画像が含まれていないことに注意してください: 約 180 または、5 つの各カテゴリに対して数十程度になります。 場合によっては、それより少なくなります。 それにも関わらず、5 つのオブジェクトの種類がかなり異なるため、このモデルは非常にうまく機能します。

では、[トレーニング] ボタンをクリックして、転移学習を開始しましょう。 Quick Training (クイック トレーニング) を選択します。 これで、複雑なビジョンモデルを通じてすべての画像を実行し、転移学習を使用して 5 つのカテゴリの予測モデルを作成しています。 これには数秒しかかかりません。非常に優れたモデルです！
確率のしきい値には、分類がまったくないことを予測する限界を設定します。 信頼度が 50% 以上の分類のみを受け入れる場合、その予測の 90.9% は正しいものになります。これが、"正確度" です。 このモデルでは、画像全体の 88.2 % が正しく分類されます。これが、"リコール" です。 アプリでは、不適切な呼び出しを行う、または呼び出しをまったく行わない許容範囲に応じてしきい値を選択します。 Tailwind Traders の場合、顧客にとって関係性が低い製品を提案することは大きな問題ではないため、低い側にしきい値を設定します。 もしこれが癌を検出するアプリのような場合は、別の呼び出しを行う可能性があります。

次に、まったく見たことのない新しい画像でモデルを試してみましょう。 これを行うには、[クイックテスト] ボタンをクリックします。 "test images" フォルダーから新しいファイルをアップロードします。 "ヘルメットを被っている男性" を試してみましょう。 予測には "ヘルメット" が表示され、確率が 99.9% であることがわかります。そのため、選択したしきい値でその呼び出しを行います。

別の画像、ドリルを試してみましょう。 このモデルでは、画像が 94.5% の確率でドリルとして識別されます。 最後に、ペンチの画像を試してみましょう。これは 99.9% の信頼度で識別されます。

したがって、モデルは 200 枚以下の画像でトレーニングされているにも関わらず、適切に動作します。
これは、潜在的なラベルを Tailwind Traders で販売されている製品のみに制限しているためです。

これで、満足したモデルができましたので、エクスポートしてアプリに組み込むことができます。 [エクスポート] ボタンをクリックすると、iOS または Android のモデルをコンテナーとしてエクスポートしたり、または、この場合はユニバーサルな ONNX 形式でエクスポートしたりできます。 これで、モデルをハード ドライブにダウンロードしました。

### <a name="slide-portable-deep-learning-models"></a>スライド:他のシステムで使えるディープ ラーニング モデル

カスタム モデルを ONNX 形式でエクスポートします。

ONNX、またはオープン ニューラル ネットワーク エクスチェンジは、Microsoft と Facebook が立ち上げたオープン標準フォーマットであり、AI モデルの無料の交換やデプロイを促進し、幅広いアプリケーションやテクノロジ ベンダーにサポートされています。

ONNX Runtime を使用して、エクスポートされたモデルを Web サイトに統合しています。

### <a name="slide-onnximagesearchtermpredictorcs"></a>スライド:ONNXImageSearchTermPredictor.cs

InferenceSession は、エクスポートされた .onnx ファイルを参照します。

モデルは、分類ラベルを生成し、検索に渡されます。

### <a name="slide-demo-onnx"></a>スライド:デモ:ONNX

デモ:ONNX のデプロイ

### <a name="video-kudu"></a>ビデオ:Kudu

[クリック] Custom Vision からエクスポートしたモデルは実際には ZIP ファイルであり、実際の ONNX ファイル、先ほど作成したニューラル ネットワークのテキスト表現である model.onnx、マニフェスト ファイルが含まれています。 

既存の Tailwind Traders Web サイトでは、products.onnx と呼ばれる ONNX ファイルのコンピューター ビジョン モデルが既に使用されています。 問題は、Tailwind Traders で販売されている製品の多くがモデルによって正しく認識されないことです。 したがって、Custom Vision からエクスポートしたばかりの、model.onnx ファイルを products.onnx という名前に変更して、Web アプリ内でそのファイルを置き換えます。これにより、トレーニングした 5 つの製品すべてが Shop by Photo によって認識されるようになります。

ここでは、Tailwind Traders Web サイトを実行する App Service リソースを Azure Portal で確認できます。 この App Service でできることは、[開発ツール] セクションにアクセスし、[高度なツール] 機能を選択します。 これにより、Kudu インターフェイスが起動します。 これで、デバッグ コンソールを使用して Web サイトのファイルシステムを参照できます。 products.onnx ファイルが配置されている、OnnxModels、W-ルート、スタンドアロン、サイトを参照してみましょう。 これは、Custom Vision で作成した新しいバージョンの products.onnx ファイルに置き換えることができます。

App Service に戻って、Web サーバーを再起動します。これにより、Shop by Photo 機能で新しい ONNX モデルが使用されるようになります。

### <a name="video-netron"></a>ビデオ:Netron

[クリック] Web サイトが再起動されるのを待っている間に、インストールしたばかりの ONNX モデルを見てみましょう。 Lutz Roeder によって開発された Netron と呼ばれる、ONNX ファイル内のニューラル ネットワークを調べることができるすばらしい Web アプリがあります。 では、products.onnx ファイルを開いてみましょう。 ここでは、モデルによって表されるニューラル ネットワークの実際のレイヤーを確認できます。 少し拡大して、上部にある入力を見てみましょう。 入力は画像です。 これは、サイズが 224x224 ピクセルの 3 枚のレイヤーからなる RGB 画像です。 実際には、ONNX ランタイムに提供する前に、ユーザーから提供された画像をトリミングしてスケールダウンする必要がありました。 これは、コンピューター ビジョン システムの視力はあまりよくなく、つまり非常に低い解像度の画像で動作しているということなのですが、非常にうまく機能しています。

次に、ネットワークで縮小してスクロールします。 Custom Vision で作成されたニューラル ネットワーク内のすべてのレイヤーを見ることができます。このコースの前半で説明したように、各レイヤーは入力画像を変換し、フィルターを適用し、出力画像を再結合します。 しかし、最終的に出力レイヤーに到達すると、出力が 5 つの値のリストであることがわかります -- これは、トレーニングした 5 つの製品 (ハンマー、ヘルメットなど) -- "loss" というラベルの付いたこの値は、モデルが各カテゴリに対して予測する信頼度です。 アプリでは、信頼度の高い要件に合わせて独自のしきい値を選択します。

Tailwind Traders の Web サイトが再起動されたので、ホームページに戻り、新しいビジョン モデルがどのように機能するかを確認しましょう。 それでは、写真をアップロードしてテスト画像の 1 つをもう一度試してみましょう。具体的には、ここまでうまく機能しなかったペンチの画像です。 確かに、これはハンマーであると考えるのではなく、Web サイトは "ペンチ" を検索し、売り出されているすべての製品を表示しています。

### <a name="slide-optimizing-app-ui-with-cognitive-services-personalizer"></a>スライド:Cognitive Services Personalizer によるアプリ UI の最適化

もう 1 つの簡単な例を次に示します。Personalizer。

"Personalizer" サービスを使用すると、ユーザーの動作から学習して、リアルタイムでアプリのインターフェイスをカスタマイズできるようになります。

### <a name="slide-recommended-screenshot"></a>スライド:候補 (スクリーンショット)

[候補] セクションでは、1 つの大きな "ヒーロー" 画像をいくつかの小さな画像と組み合わせて示します。

Personalizer は表示された [順序] セクションを選択します。

"強化学習" と呼ばれる AI 手法を使用します。

### <a name="slide-personalizer-in-action"></a>スライド:Personalizer が作動中

Personalizer は、Microsoft で長年にわたって開発されてきました。 

XBox、Bing および MSN ニュースで使用されています。

これで、独自のアプリでも Personalizer を使用できるようになりました。

### <a name="slide-reinforcement-learning"></a>スライド:強化学習

Personalizer は強化学習と呼ばれる AI 手法を実装しています。 しくみは次のとおりです。

[クリック] ユーザーに "ヒーロー" アクションを表示するとします。 [クリック] ユーザーは次の操作を行うことができない場合がありますが、[クリック] いくつかの提案を表示できます。 ゲームアプリの場合は、[クリック] "ゲームの再生"、"映画を見る"、または "クランに参加" などでしょう。 [クリック] そのユーザーの履歴やその他のコンテキスト情報 (たとえば、場所、時刻、曜日など) に基づいて、Personalizer サービスは、[クリック] 考えられるアクションをランク付けし、[クリック] 促進すべきものを提案します[クリック]。 

恐らく、ユーザーは満足するでしょう。[クリック] しかし、どうすればよいでしょうか。 これは、ユーザーが次に行うこと、および、それがやりたかったことなのかどうかによって異なります。
ビジネス ロジックに従って、[クリック] 次のように、0 ～ 1 の "報酬スコア" を割り当てます。 たとえば、ゲームをもっとプレイしたり、記事を読んだり、ストアでより多くの金額を課金したりすると、より高い報酬スコアにつながる可能性があります。 [クリック] Personalizer は、次にアクティビティを特徴付ける必要がある時のために、このような情報をランク付けシステムに提供します。

### <a name="slide-discovering-patterns-and-causality"></a>スライド:パターンと因果関係の探索

単なるレコメンダー システムではありません。

探索モードは、指定したレートで他のオプションを表示します。

リアルタイムの A/B テストと同様です。

### <a name="slide-personalizer-for-tailwind-traders"></a>スライド:Tailwind Traders 用の Personalizer

コンテキスト: 時刻、曜日、ブラウザー OS  

報酬スコア:おすすめカテゴリがクリックされた場合は 1。それ以外の場合は 0。

探索率:20%

### <a name="slide-demo-personalizer"></a>スライド:デモ:Personalizer

[クリック] 次に、動作中の Personalizer を見てみましょう。 Tailwind Traders ホーム ページに戻ってみましょう。 これまで説明していなかったことは、この候補セクションでは、製品部門の順序が Personalizer により決まるということです。
この例では、電気部門がヒーローの画像として表示されています。 Web サイトを何度も更新すると、この "探索" 動作を確認することができます。
明らかに、Personalizer は使用しているブラウザーとオペレーティング システムを使用して、この時点では、Garden Center は匿名のユーザーから最適なエンゲージメントを得ていると考えていますが、最終的にはさまざまなカテゴリを試しています。ポップアップが表示され、それを使用してエンゲージメントも測定します。

### <a name="slide-pre-built-ai-in-production"></a>スライド:運用環境で事前構築された AI

AI を運用環境に配置するための考慮事項をいくつか紹介します。

### <a name="slide-cost-considerations"></a>スライド:コストに関する考慮事項

最初の考慮事項: コスト。 

まだ Azure を使ったことがない場合は、 このリンクを使用してサインアップし、無料で $200 クレジットを取得してください。

[クリック] 開発規模のワークロードは通常無料 

[クリック] 運用量は課金

[クリック] サービスと地域別の詳細はこのリンクを参照

### <a name="slide-data-considerations"></a>スライド:データに関する考慮事項

データの送信先と使用方法について考えてみましょう。

データは推論用にアップロードされますが、使用後すぐに削除されます。 詳細については、こちらのリンクをご覧ください。

帯域幅が問題になっている場合、またはデータが規制されている場合は、コンテナーを検討してください。

### <a name="slide-deployment-with-containers"></a>スライド:コンテナーを使用したデプロイ

ダウンロード可能なコンテナーで利用できるサービスがあります。

ファイアウォールの内側にコンテナーをインストールします。データが Microsoft に送信されることはありません。

インターネット接続は請求に使用されます。 通常料金で課金されます。

### <a name="slide-ethical-considerations"></a>スライド:倫理的な考慮事項

最も重要なスライドです。

AI アプリの倫理が人々に影響を与えることを理解します。

倫理的なフレームワークがある:

ユーザーが既に行っているものをより多く達成*できる*ようにする (ユーザーを置き換えない)

あらゆるタイプのユーザーを*含める*: すべてのユーザーがアプリケーションから等しくベネフィットを得られること、および

公平さと透明性があること。

AI は、トレーニングされたデータと同じように機能することを忘れないでください。 アプリケーションがすべての潜在的なユーザーに対して動作することを確認してください。

倫理的なフレームワークが設定されていない場合は、始めるのに最適な場所は、人工知能に関する Microsoft の独自のプリンシパルであり、こちらのリンクを参照してください。

### <a name="slide-wrapping-up"></a>スライド:まとめ

事前構築されたモデルでは、すべてを行うことはできませんが、すぐに使用できるようになります。 

AI はデータで駆動されます。 常にデータを念頭に置き、うまくいかないことは何かを考えます。

実際に使ってみてください。 専門知識は必要ありませんが、倫理的影響について考えてください。

### <a name="slide-docs-alert"></a>スライド:Docs のお知らせ

ファースト ステップ ガイドとリファレンスなど、Azure Cognitive Services の詳細については、Microsoft Docs を参照してください。

### <a name="slide-ms-learn-alert"></a>スライド:MS Learn のお知らせ

Cognitive Services の使用方法について学習したい場合は、無料のコースが Microsoft Learn にあり、ステップバイステップで学ぶことができます。

### <a name="slide-resources"></a>スライド:リソース

Github リポジトリ内のすべてのリンクとコード。

AI またはデータ サイエンスにおける Microsoft 認定資格を取得したい場合は、今日の参加者のための無料の証明書を提供する特別プランをご利用ください。詳細については、こちらのリンクをご覧ください。

ご質問があれば回答させていただきます。 (そして...)

ありがとうございました。