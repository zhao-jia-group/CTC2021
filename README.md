# CIEC-CTC 2021 (Chinese Text Correction)

## 2021.06.28
增加报名成功[队伍信息](https://github.com/destwang/CTC2021/blob/main/team_info.md)，包括队伍名和codalab账号。

## 2021.06.25
训练数据已邮件发送给通过报名审核的队伍，如未收到邮件，请联系rdg_feiying@iflytek.com。
Baseline将于资格赛开始（7月1日）发布。

## 比赛介绍
文本校对任务主要是针对文本中出现的错误进行检测和纠正，属于综合性的自然语言处理研究子方向，能够比较全面体现了自然语言处理的技术水平。过往文本校对相关评测使用的都是外国语言学习者撰写的文本，这些文本的错误大多数都是一些中文母语写作者不会犯的一些错误。对于政务公文、新闻出版等行业来说，一款针对以中文为母语的用户所使用的校对系统将会有更大的帮助。因此，本赛题主要选择互联网上中文母语写作者撰写的网络文本作为校对评测数据，从拼写错误、语法错误、语病错误等多个方面考察机器的认知智能能力。

## 比赛网站
https://competitions.codalab.org/competitions/32702

## 训练数据及Baseline系统
训练数据已邮件发送给通过报名审核的队伍，如未收到邮件，请联系rdg_feiying@iflytek.com。
Baseline将于资格赛开始（7月1日）发布。

## 验证集及提交数据
验证集及数据提交格式可从比赛页面(codalab)获取，获取路径为：“Participate--File--Public Data”

其中，需要注意提交数据的格式：

1. 若句子中没有错误，则直接返回"pid, -1", 如pid=0011-2, -1

2. 若句子中有错误，则所有字段之间均以英文“,”连接，所有英文逗号的个数应为 4*n+1 个。如“pid=0011-1, 20, 别字, 轮, 论, 46, 别词, 标识, 表示,”

3. 将预测结果命名为"dev.predict"，并直接压缩为zip文件，不要保留文件夹。可参考Public Data中的submit_sample.zip

比赛页面存在拥堵情况，数据提交后可能需要一段时间才能得到评测得分。
