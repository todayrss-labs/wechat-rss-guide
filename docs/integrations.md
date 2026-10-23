<!-- Generated documentation. Please submit content corrections through Issues. -->

# 今天看啥 RSS、API 与 AI 接入

今天看啥 提供托管内容服务。本仓库公开文档与客户端示例，使用前需注册产品账号并核对对应权益。以下能力仅针对 今天看啥，不代表另一个产品具有相同接入条件。

## 选择接入方式

| 接入方式 | 当前能力 | 条件 |
| --- | --- | --- |
| RSS | 可用 | 订阅后取得个人专属地址，受账号权益与访问额度限制 |
| API | 可用 | 按接口核对会员、积分或企业权益 |
| MCP | 可用：只读工具 | 使用独立 MCP 密钥，访问有权读取的已订阅内容 |

## RSS：读取自己订阅的来源

1. 按[订阅教程](subscribe.md)取得个人 RSS 地址。
2. 使用[公共 Python 示例](https://github.com/todayrss-labs/.github/blob/main/examples/read_feed.py)，将地址保存在环境变量 `RSS_URL` 中运行。
3. 程序打印文章标题与原文链接即表示成功解析。示例只读取一次，不提供后台轮询或调度。

RSS 地址本身可能包含访问凭证，不要提交到 Git 或公开工作流配置中。纯程序读取 RSS 与 MCP 工具接入是不同方式。

## API：按业务接口获取数据

**API**：[基础 API](https://www.jintiankansha.me/about/api/basic)用于获取账号订阅列表和所订阅专栏的原始文章链接。基础 API 按当前产品说明要求 VIP-1 及以上；[扩展 API](https://www.jintiankansha.me/about/api/more_api)可按条件获取文章正文，需核对开通和积分；[高级 API 与推送回调](https://www.jintiankansha.me/about/api/adv)按企业权益及调用文档接入。购买某种权益不代表所有 API 自动可用。

1. 阅读 今天看啥 的接口说明，确认要获取订阅列表、原始文章链接还是正文。
2. 核对该接口的会员、积分或企业权益要求。
3. 在自己的账号中取得 **API 密钥**，按产品调用文档配置请求。
4. 用自己有权读取的订阅验证，成功返回目标业务数据才表示接入完成。

API 调用文档可能需要登录。具体请求地址、参数和返回字段见当前[产品说明](https://www.jintiankansha.me/about/api/basic)中的调用文档。

## AI 工具接入

**MCP / Skill**：今天看啥已发布[智能体接入指南](http://mcp.jintiankansha.me/main/start)。使用独立的 **MCP 密钥**连接支持的客户端，可以列出订阅、查询有权访问的已订阅文章并读取正文；不是全网搜索或订阅写入工具。

在 [MCP 管理页](http://mcp.jintiankansha.me/account/mcp)配置接入后，以“列出我的订阅，再读取其中一篇文章”验证。访问受主站身份、[权限与额度](http://mcp.jintiankansha.me/main/limits)限制；API 密钥与 MCP 密钥不能混用。客户端自身费用按对应产品规则执行。

## 场景说明

- **公众号集中阅读**：公众号 RSS → 阅读器分类 → 集中查看文章。
- **程序处理文章**：个人 RSS 或有权使用的 API → 程序解析 → 自己的检索或摘要流程。
- **AI 阅读订阅**：今天看啥 MCP → 查询已订阅文章 → 读取正文并总结。使用范围见接入权限说明。

上述场景描述输入与目标结果，具体自动化和 AI 客户端需自行配置。这里没有提供未经验证的导入工作流。

[返回指南](../README.md) · 事实核对日期：2026-10-23。
