<!-- Generated documentation. Please submit content corrections through Issues. -->

# 今天看啥 微信公众号 RSS 常见问题

## 账号与费用

订阅和搜索需要登录今天看啥；RSS 订阅受账号数量与有效期限制。[会员说明](https://www.jintiankansha.me/help/membership)区分免费体验、付费会员、企业权益和积分。免费体验不保证文章更新。

稳定极速订阅、历史文章同步等是按条件开通的附加服务，不能理解为购买会员后全部自动获得。价格和配额请查看当前官网及开通页面。

## 来源与内容范围

### 是否提供全文

[官网公众号教程](https://www.jintiankansha.me/about/weixin/rss_gonglue)介绍公众号全文 RSS。不同文章中的图片、排版和媒体在阅读器中的支持可能不同。Readwise 图片问题见[Readwise 相关问题解答](https://www.jintiankansha.me/about/articles/readwise#rss-images)。

### 是否需要定期扫码或自建服务

登录今天看啥、订阅并复制 RSS 地址后，即可添加到阅读器，无需定期扫码。未收录公众号仍需申请收录并等待结果。

### 能获取全部历史文章吗

不能这样理解。[历史文章同步](https://www.jintiankansha.me/about/inovation/rss_ai)仅涉及平台已有历史内容，并按条件逐步拉取，不保证补齐公众号全部历史文章。

### 是否分钟级更新

普通订阅和[稳定极速订阅](https://www.jintiankansha.me/about/weixin/fast)需分别核对。后者是按专栏开通的附加服务，改善平台更新，但阅读器仍有自己的拉取频率；本指南不承诺所有文章统一分钟级到达。

### 只想读每次推送的第一篇

查看[公众号首篇阅读说明](https://www.jintiankansha.me/about/func/weixin_first)。全局设置与个别公众号开通有不同条件，操作前核对范围和费用。

## 添加失败或没有更新

依次检查以下几项：

1. 复制的是完整的 RSS 地址，不是专栏网页地址或文章地址；避免遗漏末尾参数。
2. 登录 [今天看啥 订阅管理](https://www.jintiankansha.me/subscribe/rss/subscribed)，核对是否已订阅、权益是否有效。
3. 打开专栏，检查平台当前是否有文章；再检查源账号是否发布了新内容。
4. 手动刷新阅读器。平台获取内容和阅读器拉取 RSS 是两个环节，时间可能不同。
5. 留意账号访问额度和阅读器报错；故障未解决时[联系产品支持](https://www.jintiankansha.me/about#contact)。

反馈文档问题可使用 [Issues](https://github.com/todayrss-labs/wechat-rss-guide/issues)。不要在公开 Issue 或 AI 对话中粘贴专属 RSS 地址、API 密钥、MCP 密钥及个人账单信息。

## 可以交给程序或 AI 吗

RSS 可交给支持该格式的程序或工作流读取。API、MCP 是不同接入方式，需要分别核对权限与凭证，见[接入说明](integrations.md)。

## 可以批量迁移到另一个阅读器吗

先从产品中导出自己的 OPML，再在阅读器中导入。OPML 包含订阅地址，按个人数据保存；导出入口见[订阅教程](subscribe.md#获取-rss-地址与批量管理)，导入方法见[公共教程](https://github.com/todayrss-labs/.github/blob/main/docs/readers.md)。

[返回指南](../README.md) · 事实核对日期：2026-10-23。
