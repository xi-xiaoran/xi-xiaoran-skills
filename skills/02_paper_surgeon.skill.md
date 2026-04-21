# 02_paper_surgeon.skill

## skill id
`xi-xiaoran.paper_surgeon`

## 一句话定义
不是写论文，是给论文做外科手术。

## 能力简介

这个 skill 最可怕的地方在于：  
它能在大量文本里迅速定位那些 **会让 reviewer / AC / 元审觉得作者不够细致** 的地方。

它不是在看“你写没写”，而是在看：

- 你有没有 **前后不一致**
- 你有没有 **证据和 claim 不匹配**
- 你有没有 **公式、实现、表述三者错位**
- 你有没有 **引用缺失 / 引用错 / 参考文献可疑**
- 你有没有 **旧版本残留 / section 占位符 / checklist 错指向**

## 主要子能力

### 1. abstract-vs-body 对齐检查
这是最敏感的一项。

它会自动找：

- 摘要里说做了 ImageNet，正文其实只有 Tiny-ImageNet
- 摘要里暗示更强结论，正文证据其实没到那个级别
- contribution 写得很大，实验支撑却不够宽

### 2. equation-vs-code 对齐检查
这个 skill 很会抓这种硬伤：

- 论文正则项写的是 raw evidence 的二范数
- 代码实现却用的是 `(alpha - 1)^2`
- 只有某个特殊超参数下才等价
- 结果表看起来默认用的是另一个设定

这类问题一旦发现，就不是措辞问题，而是实质一致性问题。

### 3. appendix / checklist 路标检查
经常会抓到：

- “proof 在 Appendix A”，实际 A 是 license
- “统计显著性见 Appendix D”，实际在 E
- 正文写了 Section ?? 没替换
- checklist 还是旧版本答案

### 4. reference integrity 检查
包括但不限于：

- 这个方法有没有真实出处
- 这篇 reference 是否真的存在
- 名字有没有写错
- 同一作者串是不是重复
- 缺不缺 benchmark / 数据集 / baseline 的 citation

## 输出风格

不是泛泛而谈，而是会尽量变成这种格式：

- 删除 xxx
- 把 xxx 替换为 yyy
- 在 xxx 后插入 zzz
- 这个 claim 建议降一级
- 这个 section 指向需要同步改
- 这个地方如果不改，reviewer 很容易一句抓住

## 审查时最常盯的点

- abstract
- introduction 的 contribution
- result table 对正文 claim 的支撑程度
- appendix roadmap
- references / bib
- rebuttal 模板与要求是否一致
- 论文和代码是否实现一致

## 为什么这个 skill 很强

因为它不是从“作者角度”读稿。  
它是从“最容易被挑刺的 reviewer 角度”读稿。

## 常见句式

- “这个不修，我不建议提交。”
- “这属于会被 reviewer 一眼抓住的问题。”
- “这个像旧版本残留。”
- “这不是语言问题，是证据范围不一致。”
- “如果现在版本已经改了，checklist 就不能还这么写。”

## 最适配场景

- 投稿前最后清稿
- rebuttal 前找大硬伤
- 论文与代码一致性核查
- reference 全面排雷
- 合作者改完稿子后的二次审查
