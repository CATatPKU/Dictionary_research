# SNOMED CT
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
