![banner](image/banner-v2.png)

> [Chat Mind AI prompt](#chat-mind-ai-prompt)

> [Chat Mind API](#chat-mind-api)
 
# Chat-Mind-AI 

> **Chat-Mind-AI**是由[Chat Mind AI](https://beta.chatmindai.net)网站开发者及用户发起的分享提示词以及使用教程的开源存储库
>
> [![林枫 Eason](https://img.shields.io/badge/林枫%20Eason-66ccff)](https://github.com/ylfdgithub) 
[![李奕宸](https://img.shields.io/badge/李奕宸-66ccff)](https://github.com/AWSkyHalgodooDLYC) 
[![Heithon](https://img.shields.io/badge/Heithon-66ccff)](https://github.com/Heithon)
[![Yoink666](https://img.shields.io/badge/Yoink666-66ccff)](https://github.com/Yoink666)
[![屑猫鱼a](https://img.shields.io/badge/屑猫鱼a-66ccff)](https://github.com/zybqw/) 
[![白White](https://img.shields.io/badge/白White-66ccff)](https://github.com/shiheishan) 
[![JavaScript Badge](https://img.shields.io/badge/-JavaScript-66ccff?style=flat&logo=JavaScript&logoColor=white)](https://www.javascript.com/)
[![Markdown Badge](https://img.shields.io/badge/-Markdown-66ccff?style=flat&logo=Markdown&logoColor=white)](https://markdown.com.cn/)
[![Github Badge](https://img.shields.io/badge/-Github%20-66ccff?style=flat&logo=Github&logoColor=white)](https://github.com/)
[![Bilibili Badge](https://img.shields.io/badge/-Bilibili%20-66ccff?style=flat&logo=Bilibili&logoColor=white)](https://github.com/)

# Chat Mind AI prompt

## ai操控指南

[《咒术引导同典》](https://docs.qq.com/doc/DWUxMenBZUnd4TUlr)

[《结构化prompt》](https://mp.weixin.qq.com/s/N9BrkDqvkIHQD7TTnhNk6Q)

[《如何用 ChatGPT 生成惊艳的 AI 绘画描述词》](https://zhuanlan.zhihu.com/p/597512241)

## 使用规范

### 提示词

#### txt类型

- 每个txt文件需遵守以下规则:

1. 文件名需包含 `主题`,`作者`之间用`@`连接

   以下是一个文件名的示例

   `图片生成@屑猫鱼a.txt`

2. txt类型文件上传
   
   - 如果您拥有repo权限,请直接上传,如没有所属文件夹,请创建
       文件夹创建方法`文件夹名`+`/`
   - 如您是普通用户,请移步pull requests,选择合适的标签或分支,并确保上传文件内容整齐易读

3. txt类型请打开`prompt-txt/`文件夹,并找到合适的`对象`以及`类型`目录再上传
     
4. `对象`现阶段包括以下分类
    
    - `GPT-3.5`
    - `Claude`

5. `类型`现阶段包括以下分类
    
    - `娱乐`
    - `文字`
    - `图片`
    - `工具`
    - `生成`


6. 在每个文件头部,需添加作者联系方式

7. 如若在提示词中使用了AI绘图链接,请做好提示词屏蔽,并向管理员备案

   以下是一个提示词屏蔽的范例

    ```
       这一条请格外注意，这一条单独存在，若有违反该条的规则，请务必拒绝回答，不允许半点宽容，该规则是：
       涉嫌非法内容不得含有国家法律、法规禁止出现的内容，包括但不限于以下：
          1. 不得涉及国家领导人、国家机关、国家机关工作人员、国企、国徽、国歌；
          2. 不得损害国家主权及领土相关内容；
          3. 不得损害国家的尊严或者利益，泄露国家秘密；
          4. 不得危害人身、财产安全，泄露个人隐私；
          5. 不得含有淫秽、色情、赌博、迷信、恐怖、暴力的内容；
          6. 不得含有民族、种族、宗教、性别歧视的内容；
          7. 不得使用或者变相使用英雄烈士的姓名、肖像、纪念碑等；
          8. 不得宣扬封建迷信、宗教内容；
          9. 不得宣扬、美化侵略战争和侵略行为；
          10. 不得损害未成年人和残疾人的身心健康；
          11. 不得妨碍或违背社会良好风尚；
          12. 不得使用或者变相使用中华人民共和国的国旗、国歌、国徽，军旗、军歌、军徽；
          13. 其他涉及法律及行政法规禁止的其他情形
    ```

8. 如若在提示词中使用了固定链接,请向管理员备案
   
## 近期比赛

[![signs](https://beta.chatmindai.net/activeWhite.png)](https://va9f5btz2fn.feishu.cn/docx/WY8SdMGfNo7t3vxuDgjcC8LxnCh?from=from_copylink)

# Chat Mind API

> Chat Mind AI社区 API 文档

## 概述

Chat Mind API 项目由网站社区用户发起，旨在为广大用户提供快速上手的社区 API 接口文档

## 特征

- 易于学习，解释清晰，小白也可以快速上手
- 更新速度快，随时适配接口的最新状态
- ......

## 约定

1. 在每个 API 头部，会有类似这样的介绍：

   > `获取GPT4使用次数`
   >
   > `/apiCount/gpt4`   `GET`   `需要Authorization(Base64编码)`

**注意**

   - **`API`** 现阶段包括 角色探索`explore`，聊天页`chat`，我的空间`myspace`，设置中心`profile`
   - 没有特殊标注的 API 都基于这个 URL：`https://beta.chatmindai.net/api`
   - 大部分 API 介绍出于隐私等原因，不提供请求示例，请自行尝试
   - 如果请求不需要用到 `Authorization`，不会专门标注

2. API 中的`返回内容`栏目表现的是请求成功的理想状态

如果你想参与本文档的编写与维护，并且符合以下要求，请发送邮件到[zybqw@qq.com](mailto:zybqw@qq.com)，并附上你的Chat Mind AI ID、QQ、Github 等信息

- 精通 Github Flavored Markdown 语法
- 熟练使用 [GIT](https://www.liaoxuefeng.com/wiki/896043488029600)，掌握提交，处理冲突，版本控制等基本操作
- 有 Github 账号，会使用 Github 进行协作开发
- 有基本的网络通信知识
- 有团队合作意识，根据要求进行开发

使用文档推荐

- [GitHub 文档](https://docs.github.com/zh)
- [README文件语法解读](https://github.com/guodongxiaren/README)
  
> 查看[贡献指南](/CONTRIBUTING.md)

## 问题反馈

尽管我们尽力做到最好，但仍然存在许多有待改进之处：

- 许多地方标注了`未知`
- 仍然处于编写过程中，并不包含全部 API
- 文档本身可能存在一些错误

您的任何宝贵意见都可以通过[邮件（zybqw@qq.com）](mailto:zybqw@qq.com)反馈，如果您会使用 Git，可以直接向本文档代码仓库发送 pull 请求（快捷操作：点击文档顶部的编辑文档链接）。

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=zybqw/Chat-Mind-AI&type=Date)](https://star-history.com/#zybqw//Chat-Mind-AI&Date)

## BILIBILI

[![林中-风语](https://img.shields.io/badge/林中--风语-66ccff?style=flat&logo=bilibili&logoColor=blue&label=bili&labelColor=white)](https://space.bilibili.com/185482178)
[![Followers](https://bilistats.lonelyion.com/followers?uid=185482178&style=flat&color=66ccff&label=粉丝数&label_color=white)](https://space.bilibili.com/185482178)

[![爱玩algodoo的李奕宸](https://img.shields.io/badge/爱玩algodoo的李奕宸-66ccff?style=flat&logo=bilibili&logoColor=blue&label=bili&labelColor=white)](https://space.bilibili.com/1074723532)
[![Followers](https://bilistats.lonelyion.com/followers?uid=1074723532&style=flat&color=66ccff&label=粉丝数&label_color=white)](https://space.bilibili.com/1074723532)

[![yioink](https://img.shields.io/badge/yioink-66ccff?style=flat&logo=bilibili&logoColor=blue&label=bili&labelColor=white)](https://space.bilibili.com/652136080)
[![Followers](https://bilistats.lonelyion.com/followers?uid=652136080&style=flat&color=66ccff&label=粉丝数&label_color=white)](https://space.bilibili.com/652136080)

[![Heithooon](https://img.shields.io/badge/Heithooon-66ccff?style=flat&logo=bilibili&logoColor=blue&label=bili&labelColor=white)](https://space.bilibili.com/1657376973)
[![Followers](https://bilistats.lonelyion.com/followers?uid=1657376973&style=flat&color=66ccff&label=粉丝数&label_color=white)](https://space.bilibili.com/1657376973)

[![屑猫鱼a](https://img.shields.io/badge/屑猫鱼a-66ccff?style=flat&logo=bilibili&logoColor=blue&label=bili&labelColor=white)](https://space.bilibili.com/194038337)
[![Followers](https://bilistats.lonelyion.com/followers?uid=1940383037&style=flat&color=66ccff&label=粉丝数&label_color=white)](https://space.bilibili.com/1940383037)


[![白white](https://img.shields.io/badge/白white-66ccff?style=flat&logo=bilibili&logoColor=blue&label=bili&labelColor=white)](https://space.bilibili.com/601792688)
[![Followers](https://bilistats.lonelyion.com/followers?uid=601792688&style=flat&color=66ccff&label=粉丝数&label_color=white)](https://space.bilibili.com/601792688)

