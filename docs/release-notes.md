## 中文

本版本为 joeseesun/qiaomu-ai-rss 的 fork，移除了容量类限制，适用于订阅条目很多的大型 feed（如合并归档 feed）：

- 移除了 5 MB 的 XML 体积上限（解析、URL 下载、本地文件三处）。
- 每个源不再只读订阅文件前 200 条；不再只保留 50 篇；取消 1 MB 累计上限；单篇正文不再截断于 100,000 字符，改为保留全文。
- 取消 2,000 个个人源上限。
- 取消 20 MB 全源正文总量上限（同步时不再剥离旧源正文）与正文分片存储上限。

保留：摘要 240 字符、标题/源名长度、抓取超时与重试、刷新并发与节流、DTD/实体安全校验等。

安装：下载下方 `main.js`、`manifest.json`、`styles.css`，放到仓库目录 `.obsidian/plugins/qiaomu-ai-rss/` 下替换原文件（插件 id 未变，设置与数据保留），重启 Obsidian 后在插件列表启用。

## English

A fork of joeseesun/qiaomu-ai-rss with all feed/storage capacity limits removed for large merged feeds: no 5 MB XML cap; all items of a feed are read and kept; no per-feed 1 MB cap; full article bodies (no 100,000-char truncation); no 2,000-subscription cap; no 20 MB total body cap.

Install: drop the three files below into `.obsidian/plugins/qiaomu-ai-rss/` (same plugin id, settings preserved), then restart Obsidian.
