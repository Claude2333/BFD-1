# BFD
非洲农业不发达 所以我要支援他

# 通州区农产品信息管理系统
软件需求说明书
# 1　引言
## 1．1编写目的
说明编写这份软件需求说明书的目的，指出预期的读者。
作为一个具有7000多亩校园面积的校园，华中农业大学每年的新生以及家长还有各种游人访客可以说是络绎不绝，但是由于占地面积过大，也经常有新生和有人不知道自己的具体位置，需要问路。为了方便来访我校的访客和新生参观了解学校的景点，减轻学校导游队的负担以及导游点的设置，我们制作这个校园导航系统，提供一个校园旅游导航器来引导他们出行。
## 1．2背景 
a．待开发的软件系统的名称：华农旅游导航系统
b．本项目的任务开发者：华中农业大学地理信息科学第14实习小组
c．系统还使用ArcGIS提供的图层数据。
## 1．3定义
HZAUTGS：华中农业大学旅游导航系统
## 1．4参考资料 
a．《综合实习开发部分要求》
b．属于本项目的其他已发表的文件；
c．本文件中各处引用的文件、资料、包括所要用到的软件开发标准。 列出这些文件资料的标题、文件编号、发表日期和出版单位，说明能够得到这些文件资料的来源。
# 2　任务概述 
## 2．1目标 
本系统是一个农产品信息管理系统，主要用户为通州区的群众以及农业方面的政府工作人员。本系统可以让用户更方便的采集信息、管理信息和同步信息。
## 2．2用户的特点 
本系统为通州区的群众以及农业方面的政府工作人员提供了一个信息同步平台，用快速的计算方法、友好的界面为不同层次用户均提供了较好的服务，例如不太熟悉计算机软件操作的农民。通过简单的了解，他们能很快的熟悉操作，简洁地完成信息上传。对于希望能通过简单操作，消耗较少时间的用户来说，该系统的价值不容小觑。
## 2．3假定和约束
规定的开发期限为2016年06月23日至2016年07月15日
# 3　需求规定 
## 3．1对功能的规定
用列表的方式（例如IPO表即输入、处理、输出表的形式），逐项定量和定性地叙述对软件所提出的功能要求，说明输入什么量、经怎样的处理、得到什么输出，说明软件应支持的终端数和应支持的并行操作的用户数。 
## 3．2对性能的规定
## 3．2．1精度 
用户能够得到从指定地点到特定地点的最短路径的行走路线。 用户可以直观的得到，关键景点的信息，如：名称，描述等。
## 3．2．2时间特性要求 
响应时间：地图重要地点信息的显示能够达到即时响应；   
数据的传送与转换：完成数据的传送与转换能够达到即时响应；
## 3．2．3灵活性 
当关键景点改变时，软件适应能力，即操作方式、运行环境、同其他软件的接口、精度与有效实现无任何变化；   
校园拓扑图的编辑上，会在数据库中重新统计添加或减少的场所与其他场所的存储情况。 
## 3．3输人输出要求
输入关键景点中的某一地点，输出实际地图上的一条最短路径。目的景点的相关信息可以直观的在界面上进行输出为文字、和图像。
## 3．4数据管理能力要求 
要管理的数据有校内关键景点或这些景点所对应的拓扑结构图，以及每两个地点间的实际行走路线。对应数据库中需要关键信息点的坐标、名称、相关信息等。
## 3．5故障处理要求
某些边界点可能无法识别导致无法寻路。能够提示错误信息，稍许更改起始位置即可。
## 3．6其他专门要求
λ	实现大众普及的要求，即普适性强；  
λ	可维护性、可补充性强；  
λ	可靠性高、可读性强；    
λ	能够通过外部EXE.文件运行程序。
# 4　运行环境规定 
## 4．1设备 
操作系统为Windows的pc ；  
## 4．2支持软件 
支持软件为
## 4．3 接口
由于在Microsoft Visual Studio进行编译与测试，与其他软件无接口，所以是独立软件。
## 4．4控制 
该软件可用打包生成的外部JAR或EXE文件运行

用例
--
书写用例[编辑]
细度[编辑]
Alistair Cockburn在编写有效用例一书中确定了三种书写用例的细度。

摘要[编辑]
摘要用例有很少的句子组成来总结的用例。它十分适合在电子表格中计划软件开发。一个摘要用例能够简单插入电子表格的单元格中并且用表格中的其它列记述业务优先级，技术复杂度，版本号等。

非正式[编辑]
一个非正式的用例由文本段落组成，包括了上面提到的那些列，用总结或故事的形式详细的描述了用例。

完整正式[编辑]
一个完整正式或者复杂的用例是一个以包含了不同部分的长模板为基础的正规的文档。该用例在下面的用例模板部分进行讨论。

适当使用[编辑]
一些软件开发方法学只需要非正式的用例来定义需求。然而，开发方法学需要完整正式或详细的用例来定义需求。较大且较复杂的项目更需要使用完整正式的用例。

用例模板[编辑]
编写详细的或完整的用例，尚无通用的模板（英语：template）。现在存在很多相互竞争的模板。同时，程序员们也被鼓励用那些适合于他们的工作或者他们所做项目的模板，相对于某个指定模板的细节来说，项目的标准化要重要的多，但是这些模板的关键部分都是大体相同的，所以，虽然在某些术语上或者其他一些方面上存在不同，但是这些用例从本质上来说，是大同小异的。

典型部分包括：

用例名称
角色
描述
前置条件
事件流
基本流
备选流
后置条件
扩展点
业务规则
特别要求
迭代
不同的模板经常有其它部分，如，假设，异常流，建议，技术要求。也会有行业细节部分。

用例名称[编辑]
用例名称为用例提供了一个唯一标识。它要用动/宾格式书写，并且要充分，达到最终用户能够明白用例中描述的是什么。

迭代[编辑]
迭代部分通常需要告知读者用例完成的阶段。最初，为业务分析和确定范围的用例和用于软件开发的用例肯定会有许多不同。老版本的用例可能还在当前文档中，因为它们对不同的用户群可能会有价值。

描述[编辑]
描述部分用于在主体完成之前捕获基本场景。它提供了快速的总结，避免了读者浏览全部内容，能够很快的理解该用例的用途。

前置条件[编辑]
前置条件部分用来表达当用户开始用例时某些条件必须为真。但是它们不是启动用例的触发器。

基本流[编辑]
最低限度，每一个用例都需要描述一个主场景或者典型事件流。主事件流一般是一组有编号的步骤，如：

系统提示用户登录。
用户输入他的名字和密码。
系统验证用户信息。
系统使该用户登录入系统
……其他

备选流[编辑]
用例可能包含第二条路径，或者和主题不同的备选场景。异常或当出错时会发生什么事情也需要描述出来，这种描述可以在备选路径中或者在它本身的部分。备选路径使用基本事件流中的序号来标示在哪一点上同基本场景不同，并且如果合适它从哪一点回到基本场景中。目的是避免不必要的重复信息。

备选流的例子：

系统识别用户机器上的cookie
到步骤4（基本流）
异常路径的例子：

系统不能识别用户登录信息
到步骤1（基本流）


后置条件[编辑]
后置条件部分总结了在场景结束后事务的状态。

业务规则[编辑]
业务规则是一些成文的或未成文的规则，对于用例来说它决定了一个组织是如何执行业务的。业务规则是一个特殊种类的假定。它可能适用于某一个用例或者整个用例，甚至整个业务。

特别要求[编辑]
说明对于本用例的非功能性要求，典型的是并发情况下的响应时间要求，还有易用性要求等等
