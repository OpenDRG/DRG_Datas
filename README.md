# OpenDRG的目标是成为国家医保局CHS-DRG的开源实现，就像OpenJDK是Java SE的开源实现一样

## 资源说明
* ICD
ICD诊断、手术操作编码，各个版本的基础数据、版本之间的对照关系，以及手术操作的类别属性
  * dataset，数据集，适合计算机识别处理。每行是一条数据，用回车符分隔；每条数据是一个key-value对，用空格分隔
  * knowledge，知识库，适合人工处理。标准CSV格式，逗号分隔
* Payment
  * 各地DRG病组清单及医保支付标准
* MedicalRecord
医院病案信息、DRG分组信息、其它相关信息
  * 某统筹区三家医院病案医保分组及DRG支付信息.csv，分组规则为CHS-DRG 1.1（628组），医院A是三级医院，其它两家是二级医院，一共约21万条记录，可用于分析不同等级医院的DRG支付盈亏趋势
  * 某中医院病案按CHS-DRG分组结果及中医病证信息.csv，分组规则为CHS-DRG 1.1（628组），约6万条记录，可用于分析CHS-DRG分组与中医病证的关联性，进一步完善分组方案
  * 某三级综合性医院国考病案数据2020-2022.csv，约16万条记录，数据格式：HQMS标准格式，文件编码：iso-8859-1编码（中文需转换后才能正常显示）
**病案已除去个人及医院敏感信息，但仍属于医院真实业务数据，仅供分析研究，不得转发扩散，引发任何后果责任自负**

## 联系开发团队
请发邮件至14463966@qq.com