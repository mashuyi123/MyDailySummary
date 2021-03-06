编写完善checklist目的
---------------
维护一套checklist，借鉴测试，减少常规测试和常规bug。

提测说明
----
新增模块
修改模块
影响范围
测试注意事项等。

前端：
---
 - 代码是否提交完整
 - 代码是否提交了与本次新增/修改无关的内容
 - 界面控件标题是否正确
 - 界面提示信息是否准确
 - 界面控件必填项检查（null，空格等）
 - 界面布局合理性检查
 - 下拉框选择项检查
 - 文本输入框检查（最大最小字符数等长度限制，输入超长字段，输入框是否被撑开）
 - 输入合法性检查（文本OR数值，是否支持小数）
 - 联动关系检查（地区等有层级关系的数据）
 - 导入文件格式检查（不合理的文件格式是否有提示）
 - 导出文件结果是否正确（是否按查询条件导出，导出数据格式是否正确）
 - 按钮功能是否实现（重置/取消/是否跳转等）
 - 查询操作显示结果是否符合常规（日期格式，金额，排序等）
 - 分页检查
 - F12控制台是否有error
 - 切换窗口大小，页面是否按比例缩放（前期可不做）
 - 浏览器的前进、后退、刷新按钮，系统是否正确处理（前期可不做）
 - 是否进行过自测或冒烟测试

后台：
---
 - 代码是否提交完整
 - 代码是否提交了与本次新增/修改无关的内容
 - 提测模块主流程是否通畅
 - 提测模块是否进行异常情况处理（空指针等）
 - apizza上文档是否和代码保持一致
 - 是否进行过自测或冒烟测试


数据库：
----
 - 新建的数据库表（提供表名或者SQL脚本文件）
 - 修改的数据库表结构（表名，变动内容）
 - 寄存数据是否需要脚本修改

测试
--
**新功能测试：**
	大颗粒度保证各个功能点被覆盖，不必过于详细，进行持续验证；功能满足后进行bug大扫除，细粒度验证。

**回归测试：**
 通过code diff了解代码变动的地方，做关联分析，明确哪些地方需要回归测试。
 回归测试主要保证功能点没有问题，忽略细节问题。
 为各系统维护一套测试点的checklist，精简列出需要关注和易被遗漏的测试点，可以放到wiki，不断补充完善。
 