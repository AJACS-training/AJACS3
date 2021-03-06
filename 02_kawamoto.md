[[AJACS3]]

        --
目次

#contents
        --

#  生命科学データベース横断検索の利用法 [#xbd5b6cf]
> http://lifesciencedb.jp/

横断検索サービスは国内外の有用なデータベースや文献を一括して検索するサービスです。各データベースの情報はオリジナルのサイトにおいたまま、検索に必要な情報をクロウリングやオリジナルデータを使って作製します。いわばGoogleのような検索です。検索エンジンはHyper Estraierを使っています。このエンジンは現在mixiの検索などに使われているオープンソースのプログラムです。統合DBセンターでは約20ノードで構成されるクラスターサーバーで計算をさせています。
## 1 横断検索に収録されているデータベース [#l28fd7fb]
現在横断検索に収録されているデータの一覧は[[横断検索収録DB一覧:http://lifesciencedb.jp/dbsearch/dblist.html]]で見ることができます。それぞれのデータベースの属性にあわせて画面の左側にグループごとにわけて検索結果が表示されるようになっています。
###  1-1 日本語文献 [#j0834d51]
::[[蛋白質核酸酵素:http://www.kyoritsu-pub.co.jp/pne/]]|共立出版の生命科学の総説誌。創刊約53年の歴史を持つ。基礎的な話題を幅広くとりあげる。日本語の総説はなかなか業績にはなりにくいかもしれないが、選ばれて書けるのは誇りだし、何より他の人にわかってもらうにはやはりまずは日本語。
::[[毎日新聞:http://www.nichigai.co.jp/sales/mainichi/mainichi-series.html]]|CDによって提供される毎日新聞のテキストデータを使った過去記事の検索。オンライン上のニュースは一定時間がたつと消滅してしまうので、過去のニュースを探す時に便利。
::[[文科省「ゲノム」研究報告書:https://www.genome-sci.jp/]]|文部科学省の特定領域研究のうち「ゲノム」と呼ばれる領域の報告書を集めて検索できる。科学研究費には種別が色々あるが、重点的な課題はこのように大きなグループで進められる。つまり重要な成果が報告書にはたくさん記載されていると思われるので、それらを集めて一括して検索できるようにするのが目標。
###  1-2 特許 [#td98c118]
::日本特許　公開広報 | 特許権が認められた発明のデータ
::米国特許（外部情報）|アメリカの特許。機械的な大量ダウンロードは禁止されているので検索は米国特許庁のシステムに質問を投げている。
::欧州特許 (外部情報）|ヨーロッパの特許。米国特許と同様。
###  1-3 用語解説 [#c31c587f]
::[[ウィキペディア:http://ja.wikipedia.org/wiki/]]|オンライン百科事典。英語版が中心だが全部で264言語ある。英語版には250万の記事、日本語版にも50万近い記事がある。誰もが自由に編集に参加できる。最初は記述の正確性に欠けるのではと言われていたが、ネイチャーにブリタニカ百科事典と比較しても劣らないという調査結果が報告されたりした。
###  1-3 基本のデータベース [#iafff6d5]
::[[KEGG:http://www.kegg.jp/ja/]]|Kyoto Encyclopedia of Genes and Genomesの略。生命システム情報統合データベース。京大化学研究所および東大医科研の金久研究室によって構築されている世界的に有名なデータベース。遺伝子配列を中心に論文から関連する記述を抽出しパスウェイやリンクとして再構築し知識として体系づける。統合データベースプロジェクトでは後述する医薬に関する薬や化合物の統合を担っている。
::[[PDBj:http://www.pdbj.org/index_j.html]]|Protein Data Bank Japan の略。生体高分子の立体構造データベースの日本アーカイブ。国内の登録を受け付けるとともに、日本語のドキュメントも整理されている。今年、登録された立体構造が５万を超えた。
::[[RefSeq:http://www.ncbi.nlm.nih.gov/RefSeq/]]|Reference Sequenceから命名された。GenＢankへの登録数が増えredundancyが問題になってきたため、重複の無い基準となる配列のコレクションを作った。現在リリース２９で５千以上の生物種にわたって５００万以上の蛋白質がコレクションされている。
::[[OMIM:http://www.ncbi.nlm.nih.gov/omim/]]|Online Mendelian Inheritance in Manの略。ヒトの遺伝子と遺伝病のカタログ。
###  1-4 生物種ごとのデータベース [#n10c4362]
+ヒト、動物
::[[H-Inv:http://www.jbirc.jbic.or.jp/hinv/ahg-db/index.jsp]]|ヒト遺伝子アノテーションデータベース。ヒトの遺伝子と転写産物を対象とした統合データベース。ヒトゲノム上の遺伝子に対してcDNAを基準にして様々な情報を注釈付けするプロジェクト。産業技術総合研究所。
::[[JSNP:http://snp.ims.u-tokyo.ac.jp/index_ja.html]]|日本の一塩基多型(SNPs)のデータベース。理化学研究所と東大医科研によりミレニアムプロジェクトやオーダーメイド医療実現化プロジェクトで測定されたデータが中心。最近はDNAチップにより解析されている。データそのものはA, G, C, T の塩基の情報だが、正しく理解するには遺伝学の知識も必要。
::[[DBTSS:http://dbtss.hgc.jp/]]|転写開始点及びプロモーター領域に関するデータベース。完全長cDNA配列の5'末端の情報が中心。現在では次世代シーケンサーも利用されている。東大医科研。
::[[HUGE:http://www.kazusa.or.jp/huge/index.html]]|ヒト長鎖 cDNA (KIAA cDNA) 解析情報データベース。かずさDNA研究所。
::[[NEDO:http://www.kazusa.or.jp/NEDO/index.html]]|ヒト長鎖 cDNA (FLJ cDNA) 解析情報データベース。かずさDNA研究所。
::BodyＭap|ヒトの臓器ごとの遺伝子発現を観測したデータベース。ESTという短い遺伝子配列の解読法を生み出した。現在実験データの追加はされていないが、発現データの統合データベースとして更新されいてる。
::[[FANTOM:http://fantom.gsc.riken.go.jp/index.html]]|Functional Annotation of the mouseの略。マウス遺伝子の機能情報に関するデータベースで現在のバージョンはFANTOM3。FANTOM1および2はcDNAの機能に関する注釈が中心であったが、現在ではCAGEのデータが公開されており、RNA mappingのデータとしても利用価値が高い。京大の山中教授が万能細胞を作るときに参考にしたデータベースとして話題になった。
+植物
::[[CLOVER:http://clovergarden.jp/]]|クローバーとマメ科植物を対象とした、ゲノム情報とゲノム研究用リソースのデータベース。かずさDNA研究所。
::[[RAPDB:http://rapdb.dna.affrc.go.jp/]]|Rice Annotation Project Databaseの略。イネゲノム上の全遺伝子の構造と機能の人手によるアノテーション。農業生物資源研究所。
::RPSD|イネ、トウモロコシ、小麦等の植物のタンパク質構造データベース
+微生物
::[[CYANOBASE:http://bacteria.kazusa.or.jp/cyanobase/]]|シアノバクテリア（藍藻）ゲノムデータベース。（午前中の講義で紹介がありました。）
::RHIZOBASE|根粒菌のゲノムデータベース。かずさDNA研究所。
::[[GTOP:http://spock.genes.nig.ac.jp/~genome/gtop-j.html]]|ゲノムにコードされる全タンパク質の配列データを解析した結果をまとめたデータベース。配列相同性解析を主な手段として、立体構造の情報を積極的に利用していることが特徴
::Mycoplasma penetrans genome|マイコプラズマのゲノムデータベース。マイコプラズマは細胞壁やアミノ酸合成経路を持たない細菌。真核生物の細胞に共生する。ゲノムサイズは小さい。
+医薬
::[[ゲノムネットJAPIC:http://www.genome.jp/kusuri/]]|日本医薬情報センター(JAPIC)の医薬品添付文書情報とKEGG DRUGを統合したデータベース。
::[[OMIM:http://www.ncbi.nlm.nih.gov/omim/]]|Online Mendelian Inheritance in Manの略。ヒトの遺伝子と遺伝病のカタログ。
+糖鎖、脂質関連
::[[GGDB:http://riodb.ibase.aist.go.jp/rcmg/ggdb/]]|糖鎖に関連する遺伝子（糖転移酵素遺伝子など）の各種情報についてのデータベース
::[[LipidBank:http://lipidbank.jp/]]|整理活性脂質データベース。脂質に関するデータを化合物ごとに整理しデータベース化。
+海外
::EntrezＧene|
::RefＳeq|
::PIR|
::OMIM|
###  1-5 これから増えるデータベース [#uf91bbe0]
- 特許・実用新案広報|特許出願後1年6ヶ月後に公開された発明の内容
- [[理研のデータベース群:http://www.riken.go.jp/index_j.html]]
- 微生物系データベース
- 医薬系系データベース
#br
国内だけでも300にのぼるデータベースがあります。今後はこれらの中から役に立つものを順に追加していきます。

##  横断検索の機能（使い方） [#o00876e7]
実験医学（羊土社）の最新号、特集創薬の新規ターゲットにつながる「メタボリックシンドロームの鍵因子」を題材に実際に検索をしてみます。
#ref(http://www.yodosha.co.jp/book/book_img_detail/9784758100373.jpg)
- 「PPARrとWntシグナルを標的とした老化・生活習慣病病態解析」という総説には、分子の名前や病名、をはじめたくさんの重要な概念が含まれていますが、生命科学の研究は今やこのように非常に多角的になっています。
- 総説の要旨には「PPARγは脂肪細胞分化や糖・脂質代謝制御を担う鍵因子の一つであるが、骨代謝における機能も近年報告されている」と書かれていますがPPARを理解するには非常に多くのことを理解しなくてはなりません
- そこが横断検索の出番です。


# 実習　それではみなさんも実際にキーワードを入力して検索してみましょう [#k9aa1faf]

## 検索の基本 [#j1ca5011]
- (1)アルツハイマー　と入力してみましょう。アルツハイマーが英語に翻訳されて検索されます。あらゆる単語を翻訳するわけではありませんが、綴りのわからない病名などを検索するときには便利です。
## データベースによる絞り込み [#y81b9c37]
+(1)画面左側にあるデータベースのうち、文献の矢印を押してみましょう
+(2)ここでは毎日新聞過去記事をクリックしてみます。
+(3)検索結果は毎日新聞のみになります。
## 遺伝子名による絞り込み [#xf8e9f6e]
アルツハイマーを遺伝子名に含む遺伝子のリストが上部のボックスに表示されています。調べたい遺伝子がわかっているときには遺伝子名をクリックすると、遺伝子ＩＤを手がかりに関連するエントリーが絞り込まれます。
+(1)遺伝子名をクリックしてみましょう。
## 検索式による検索 [#jcfa765c]
::検索語句を、ページ右上にある検索窓に入力してください。もし、"インスリン"という単語を含む文書を検索したいなら、次のように入力して下さい。|インスリン

::"インスリン"および"糖尿病"の両方を含む文書を検索したいなら、空白で区切って次のように入力して下さい。AND検索といわれるものです|
インスリン 糖尿病
::"インスリン"または"インシュリン"のどちらかが含まれる文書を検索する場合には、｜で区切って次のように入力して下さい。|
インスリン | インシュリン
::"インスリン"を含み"like"が含まれない文書を検索する場合には、！で区切って次のように入力して下さい。| インシュリン ! like	　 	　 	　 	　 	　 	　 	　 	　 	　 	　
 "| "は、スペース ・ "!"よりも優先度が高くなっています。
このような検索を検索式とか検索条件式とかいいます。空白のかわりにANDを使ったり、ORを使ったりするのも一般的です。検索式を使うと色々高度な検索を行うことができます。NCBIのEntrezなどでやってみてください。
## firefoxの検索プラグインに横断検索を追加してみましょう [#q99c92f8]
さきほどのコンピューターの使いこなし術の復習です。自分でやってみましょう。

&smile;横断検索の使い方は統合TVの番組-「統合ホームページ」を使い倒す－[[横断検索:http://togotv.dbcls.jp/20080603.html#p01]]-で復習できます。
