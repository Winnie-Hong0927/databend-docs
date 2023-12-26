---
title: 使用 Dashboard
---

Dashboard 用于通过各种图表类型（包括记分卡、饼图、柱状图和折线图）展示查询结果。这些图表是根据查询结果生成的。在工作表中执行查询后，您可以选择基于查询结果创建图表。刷新 Dashboard 允许您重新执行与图表对应的查询，从而使用最新的结果更新图表。

![Alt text](@site/static/img/documents/dashboard/dashboard.png)

在 Databend Cloud 中，您可以根据需要创建多个仪表板。一个仪表板可以包含一个或多个图表。每个图表对应一个特定的查询结果，但可以被集成到多个仪表板中。

创建 Dashboard 步骤如下：

1. 在工作表中运行一个查询，您将使用此查询结果生成一个图表。

2. 在结果区域，点击“图表”选项卡。

![Alt text](@site/static/img/documents_cn/dashboard/chart-btn-cn.png)

3. 在“图表”选项卡上，从右侧的下拉菜单中选择一个图表类型。接下来，使用下拉菜单列表下方的“数据”和“样式”选项卡中的选项，指定数据并自定义图表的外观。

以下聚合函数帮助您从查询结果的原始数据中进行总结并揭示有价值的模式。请注意可用于聚合的函数会根据您选择的不同数据类型和图表类型而变化。

| 聚合函数 	| 描述                                                   	|
|----------	|--------------------------------------------------------	|
| None     	| 数据不做任何改动。                                     	|
| Count    	| 计算查询结果中字段的记录数量（不包括包含 NULL 和''的记录）。 	|
| Min      	| 计算查询结果中的最小值。                               	|
| Max      	| 计算查询结果中的最大值。                               	|
| Median   	| 计算查询结果中的中位数。                               	|
| Sum      	| 计算查询结果中数值的总和。                             	|
| Average  	| 计算查询结果中数值数据的平均值。                       	|
| Mode     	| 鉴定查询结果中出现频率最高的值。                       	|


4. 返回 Databend Cloud 主页并在左侧导航菜单中选择“Dashboard”，然后单击“新建 Dashboard”。

5. 在新建的 Dashboard 中，单击“添加图表”。将图表从左窗格拖放到仪表板上。如果左侧窗格中有多个可用图表，请随意拖动所需数量的图表。

:::important
从工作表中的查询结果生成图表后，请不要在同一工作表中运行其他查询，因为这样做会导致图表在 Dashboard 上不可用。
:::