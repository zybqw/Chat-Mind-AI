# Chat Mind API

> Chat Mind AI 社区 API 文档

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
   > `/apiCount/gpt4` `GET` `需要Authorization`

2. API 中的`返回内容`栏目表现的是请求成功的理想状态
   > 理想返回数据一般为 `{code: 200, reason:"some reason",data:[]}`

**_注意_**

- **`API`** 现阶段包括：
  - 角色探索`explore`
  - 聊天页`chat`
  - 我的空间`myspace`
  - 设置中心`profile`
  - 创建角色`create`
  - 登录 `login`
- 没有特殊标注的 API 都基于这个 URL：`https://x.chatmindai.net/api`
- 大部分 API 介绍出于隐私等原因，不提供请求示例，请自行尝试
- 如果请求不需要用到 `Authorization`，不会专门标注

如果你想参与本文档的编写与维护，并且符合以下要求，请发送邮件到[zybqw@qq.com](mailto:zybqw@qq.com)，并附上你的 Chat Mind AI ID、QQ、Github 等信息

- 精通 Github Flavored Markdown 语法
- 熟练使用 [GIT](https://www.liaoxuefeng.com/wiki/896043488029600)，掌握提交，处理冲突，版本控制等基本操作
- 有 Github 账号，会使用 Github 进行协作开发
- 有基本的网络通信知识
- 有团队合作意识，根据要求进行开发

使用文档推荐

- [GitHub 文档](https://docs.github.com/zh)
- [README 文件语法解读](https://github.com/guodongxiaren/README)

> 查看[贡献指南](/CONTRIBUTING.md)

## 问题反馈

尽管我们尽力做到最好，但仍然存在许多有待改进之处：

- 许多地方标注了`未知`
- 仍然处于编写过程中，并不包含全部 API
- 文档本身可能存在一些错误

您的任何宝贵意见都可以通过[邮件（zybqw@qq.com）](mailto:zybqw@qq.com)反馈，如果您会使用 Git，可以直接向本文档代码仓库发送 pull 请求（快捷操作：点击文档顶部的编辑文档链接）。
