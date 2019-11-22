# SNOMED CT (Systematized Nomenclature of Medicine -- Clinical Terms）
### 概述
SNOMED CT是广泛的临床术语，由SNOMEDRT®(reference terminology)和英国国家卫生服务（NHS）临床术语(readcodes)于2002年合并，扩展和重组形成。它提供英语（或任何语言）最全面的临床词汇。其用途也从最初满足以病理学术语为主体内容的分类和检索扩展为能够满足信息化时代临床信息系统的检索、数据汇聚、分析和交互共享。
SNOMED CT在医疗保健信息技术标准小组制定的互操作性规范中已被指定为电子健康信息交换的美国标准。并且已被美国联邦政府通过综合健康信息学（CHI）计划采用，用于多个临床领域。2007年4月，国际卫生术语标准制定组织（International Health Terminology Standards Development Organization,IHTSDO）收购了SNOMED CT。自2007年以来，成员国的数量已从9个增加到29个。（无中国）IHTSDO的成员可以是国家政府的机构，也可以是由其所代表的国家/地区中适当的国家政府机构认可的其他机构（例如公司或区域政府机构）。成员国承诺在其管辖范围内传播IHTSDO术语，包括在适当情况下创建本地翻译。


## 呈现形态和交互模式
SNOMED CT浏览器提供浏览和查询医学术语集的方法，它默认Google Chrome运行，使用IE浏览器可能会造成错误。同时它还提供了REST API,但官网提示在医疗卫生生产系统中滥用API可能导致封号。

![browser](https://github.com/chiris-ye/Dictionary_research/blob/master/image/browser.PNG)

我们可以看到，SNOMED CT浏览器提供了国际版和成员国版的医学术语集，因为中国并未参与SNOMED CT，我们在利用SNOMED CT进行翻译时应选择国际版进行查询。

打开国际版浏览器点击左侧窗口的Taxonomy标签我们可以查看到SNOMED CT依据现代西医学本体论疾病观将所有概念分为19个顶级类，全面覆盖了临床科研工作所需的概念种类，各类之间具有不同的逻辑关系，通过“Is—A”关系建立类之间的等级体系，其中“临床发现”(clinical finding)与“操作”(procedure)是核心类，其他类为“支持性类”。

![taxonomy](https://github.com/chiris-ye/Dictionary_research/blob/master/image/taxonomy.PNG)

![taxonomy_01](https://github.com/chiris-ye/Dictionary_research/blob/master/image/taxonomy_01.PNG)

用户可以像使用搜索引擎一样再搜索框中输入想要查询的术语信息，且浏览器提供完整匹配和部分匹配的选择。

![search_box](https://github.com/chiris-ye/Dictionary_research/blob/master/image/%E6%90%9C%E7%B4%A2%E6%A1%86.PNG)

例如我们在翻译“高烧不退”相关的医学领域文章时，其中介绍了多种类型的“高热”病症，利用英汉词典进行翻译可能存在专业性不强，且多组医学概念易混的问题。而如果利用搜索引擎进行查询，得到的无效信息过多，译者需要划分过多的时间在知识阅读和语料筛选上。而利用SNOMED CT则能够很好地缩小我们需要查看的资料范围，并且得到的译文具有很强的权威性。

![fever](https://github.com/chiris-ye/Dictionary_research/blob/master/image/fever.PNG)

在这里我们可以根据括号中的文字，判断哪些是发现（finding），哪些是疾病（disorder），哪些是有机体（organism）。因为我们确定翻译对象为疾病，我们可以在左侧选择只显示disorder相关内容，在图中我们看到了熟悉的Drug fever和Zika fever。原文中描述了由花粉过敏引起的花粉热，但是我们并没有看到有“pollen fever”这种病症，我们查看一下每个概念右侧对应的描述，发现hay fever的描述非常像我们要找的花粉热。我们点击查看具体内容。

![hay_fever](https://github.com/chiris-ye/Dictionary_research/blob/master/image/summary.PNG)

在这里，它提供了一些相关信息，根据Is-A关系，花粉热的父类为：Allergic disorder caused by substance (disorder)和Seasonal allergic rhinitis (disorder)，子类为： Allergic rhinitis caused by grass pollen (disorder)、Allergic rhinitis caused by tree pollen (disorder)和Allergic rhinitis caused by weed pollen (disorder)，这样可以对疾病的纵向结构有更为清晰的认知。语义关系与连接概念”方法的应用,明确了每一个概念在知识体系中拥有的与其他概念纵向及横向的语义关系，实现了概念的逻辑化定义。概念逻辑化定义与仅通过术语定名加上文字解释这种概念定义方法相比结果更为精确,能够有效避免术语在实际应用中由于脱离了文字解释便无法被正确理解的弊端,从而保证了临床信息在捕获、传递、存储、利用等工作环节的数据质量，为标准化术语应用提供了极大便利。而且还提供了疾病本身的相关信息，如临床病程为季节性、相关形态学为发炎、过敏原为花粉等，帮助我们对这一概念有更多的了解。为了更清晰地查看相关条目我们可以跳到diagram标签。

![diagram](https://github.com/chiris-ye/Dictionary_research/blob/master/image/diagram.PNG)

我们再点击detail标签，我们可以查找美国和英国再医学领域使用“花粉热”这一医学术语时最常使用的英文术语，我们可以发现其实“hay fever”的接受度不如“Allergic rhinitis caused by pollen”，因此我们更建议将“花粉热”翻译成“Allergic rhinitis caused by pollen”。

![detail](https://github.com/chiris-ye/Dictionary_research/blob/master/image/detail.PNG)

## 第二题（垚鑫）
### 多模态
传统的电子词典只是将纸质词典上已有的内容电子化，并没有增加新的内容或形式。由于纸质词典通过纸这一介质呈现内容，内容的形式局限在文字和图片，而基于印刷成本考虑，许多纸质词典很少提供高质量的彩色图片。这样一来，常规电子词典如果只是将纸质词典的内容通过屏幕显示出来，就未能最大程度地发挥计算机的优势。
新时代的电子词典，除了提供传统电子词典所能够提供的文字和图片外，还可以提供音频和视频，乃至虚拟现实或增强现实的体验，让词典使用者身临其境地体验词汇的使用

### 联合查询
传统的电子词典由词典出版社开发，每部词典都对应一个独立的软件（电脑上）或应用程序（手机上）。因而，词典使用者想要查找一个单词，需要先自行确定这个单词在哪部词典中，然后打开相应电子词典进行查询。
新时代的电子词典，应该具备联合查询的功能，一次检索，可以查看该单词在多部词典中的释义。另外，词典使用者应该可以自行设置联合查询的分组，将不同词典加入不同分组中，以应对不同用途。例如，将与医学有关的词典加入某分组，以方便进行医学翻译。

### 取词
传统的电子词典使用起来局限在软件内部，无法在网页浏览器、文本编辑器中取词。
新时代的电子词典应该具有良好的兼容性，可以在其他软件中获取单词进行快速查询。

### 更新换代
传统的电子词典更新换代慢，是在纸质词典出版时，同步发布的和纸质词典内容一致的电子化词典。
新时代的电子词典应该具有实时更新的能力，以应对新单词、新释义、新例证的需要。

### 全文检索
传统的电子词典检索方式与纸质词典类似，都只能按已有词头进行查找，无法查询释义中出现的内容。
新时代的电子词典应该具有全文检索的功能，方便查找释义中的内容。

### 反向查询
传统的电子词典仅是由某一语言向另一语言的词典，无法通过该词典生成可以反向查询的词典。
新时代的电子词典应该可以从一部词典生成可供反向查询的词典。

### 高级检索
新时代的电子词典应该可以通过正则表达式或类似形式对单词、词组或句子进行复杂的查找和匹配。

### 用户体验
新时代的电子词典应该提供更好的用户体验，如快速复制释义内容、收藏单词的某项释义，根据使用情况对词典顺序进行更好的排列。

### 数据同步与共享
新时代的电子词典应该将用户数据在多设备上无缝衔接，亦可方便地与他人共享知识。
