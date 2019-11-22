### 语言系统研究
#### 一体化医学语言系统 UMLS
英语：Unified Medical Language System，又称为统一医学语言系统，是对生物医学科学领域内许多受控词表的一部纲目式汇编。UMLS提供的是一种位于这些词表之间的映射结构，使这些不同的术语系统之间能够彼此转换；同时，UMLS也被看作是生物医学概念所构成的一部广泛全面的叙词表和本体。UMLS还进一步提供有若干适用于自然语言处理的工具。UMLS主要旨在供医学信息学领域的信息系统开发人员使用。
https://zh.wikipedia.org/wiki/%E4%B8%80%E4%BD%93%E5%8C%96%E5%8C%BB%E5%AD%A6%E8%AF%AD%E8%A8%80%E7%B3%BB%E7%BB%9F

UMLS由下列组件构成：
(1)超级叙词表(Metathesaurus),是UMLS知识源的核心,由来自各种受控词表的概念和术语以及它们之间的关系所构成;
(2)语义网络(Semantic Network),是对超级叙词表概念的分类和分类之间的关系;
(3)专家辞典(SPECIALIST Lexicon),是一个词典信息库,用于自然语言处理;
(4)支持性的软件工具,各种利用UMLS的工具和程序。
据统计,超级叙词表是最经常被使用到的知识源,约占总使用量的94%;其次是语义网络和专家词典与工具,约占使用量的28%;三项都使用的用户占全部用户的19%。
《UMLS及其在智能检索中的应用》
http://manu44.magtech.com.cn/Jwk_infotech_wk3/article/2012/1003-3513/1003-3513-28-4-1.html

#### SNOMED CT
Systematized Nomenclature of Medicine - Clinical Term的缩写，全称是医学系统化命名-临床术语

SNOMED CT（Systematized Nomenclature of Medicine -- Clinical Terms，医学系统命名法－临床术语，医学术语系统命名法－临床术语），是一部经过系统组织编排的，便于计算机处理的医学术语集，涵盖大多数方面的临床信息，如疾病、所见、操作、微生物、药物等。采用该术语集，可以协调一致地在不同的学科、专业和照护地点之间实现对于临床数据的标引、存储、检索和聚合。同时，它还有助于组织病历内容，减少临床照护和科学研究工作中数据采集、编码及使用方式的变异。
组成
- 概念表
- 描述表
- 关系表

概念和描述：每个唯一性数字型代码、唯一性名称（全称，即Fully Specified Name）和描述（包括一条首选术语和一条或多条同义词）所指定的基本含义单位。 SNOMED CT不再使用词条表的方式对术语进行表示，而是采用概念的形式。概念以理解为医学中标准的临床术语，每个概念都有唯一的概念码，但每一个概念都可能有多个描述，并且由993420条描述形成了庞大的描述表——我们可以理解成同义词表。如“Pain in throat”（咽喉痛），在SNOMED CT中是概念，而在实际应用中，它将会有多种不同的术语表达，如“Sore throat”、“Throat pain”、“Pain in pharynx”、“Throat discomfort”、“Pharyngeal pain”、“Throat soreness”，但它们并不是概念，而只作为描述被收集在描述表中。每一条概念有若干描述与之对应，描述表中的每一条描述也有与之相对应的概念存在。

SNOMED CT 中共有3种术语描述类型，即“指定全称”（Fully Specified Name，FSN）、“首选术语”（Preferred）及“同义术语”（Acceptable）。每个概念都有一个“指定全称”和一个“首选术语”，同义术语是除去首选术语外，其他能够描述FSN所描述概念的术语.
例子：
概念 Myocardial infraction 22298006
规范化全称：Myocardial infraction(disorder) DescriptionID 751689013
首选术语：Myocardial infraction DescriptionID 37436014
同义词：Cardiac infarction DescriptionID 37442013
同义词：Heart attack DescriptionID 37443015
同义词：Infarction of heart DescriptionID 37441018

关系：用于在同一层级结构之内或不同层级结构之间将不同的概念联系起来。 SNOMED CT中的概念与概念间是有一定“关系”存在的。概念有36万条，但关系有近146万条。这种基于概念间的语义关系令数据的获取充分可靠。在SNOMED CT中，关系分为两种: IS-A关系与属性关系。

IS-A在同一个层面中，表示某些概念间的关系。如关节炎属于关节系统疾病，而关节系统疾病属于骨科疾病，这样关节炎→关节系统疾病→骨科疾病就形成了一种IS-A关系;

属性关系表示跨层面的概念间的关系。
例子：
“阑尾炎”是一种疾病，但从形态学上看，“阑尾炎”属于炎症的一种，在属性关联中，可由“阑尾炎”引导出“炎症”。

attribute（属性）关系

临床发现 手术/操作 事件 身体结构 药物/生物 制品、设备、标本等各类概念均有其特有的属性

临床发现：发现的部位、形态学表现、与其他（如原因）的关系、严重度、临床进程等

手术/操作：手术部位，手术目标部位，手术方法，手术路径，手术用药，优先度


