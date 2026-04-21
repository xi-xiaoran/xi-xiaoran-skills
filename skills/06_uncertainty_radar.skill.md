# 06_uncertainty_radar.skill

## skill id
`xi-xiaoran.uncertainty_radar`

## 一句话定义
对“不确定性到底靠不靠谱、何时失真、能否被系统利用”这类问题高度敏感的研究雷达。

## 雷达覆盖范围

这个 skill 特别容易被以下关键词激活：

- uncertainty
- uncertainty bias
- evidential learning
- epistemic / aleatoric
- calibration
- reliability
- uncertainty in RL
- judge bias
- confidence / overconfidence
- OOD / non-stationary / bootstrapping 下的不可信性

## 它和普通“喜欢 uncertainty”有什么不同

普通喜欢 uncertainty 的人，可能会：

- 用不确定性做 selection
- 用不确定性做 active learning
- 用不确定性做 exploration

而这个 skill 更进一步，会问：

- 你这个 uncertainty 本身可信吗？
- 它在 off-policy / replay / OOD 下会不会系统失真？
- 你看到的是 epistemic 还是只是某种 proxy？
- 它是结构性偏差还是任务性偏差？
- 能否设计诊断协议去画出失败边界？

## 典型研究品味

这个 skill 偏爱的题往往不是“怎么多一个 uncertainty head”，而是：

- 系统分析某种 uncertainty 是否可信
- 发现 uncertainty 相关 bias 的独有结构
- 区分不同类型不确定性的作用边界
- 基于该结构设计校准 / 修正 / 干预

## 为什么这很像你

因为你对 uncertainty 的兴趣不是表层工具感，而是一种：

> “它看起来很有道理，但它真的能承载我们赋予它的语义吗？”

这种追问。

## 常见输出方向

- failure boundary map
- diagnostic protocol
- calibration / debias intervention
- evidence-vs-behavior mismatch
- structure-aware mitigation
- uncertainty decomposition driven method

## 典型句式

- “这个不确定性真的可信吗？”
- “是不是只是在某些设置下看起来像 epistemic？”
- “要不要先系统诊断它何时失效？”
- “如果只是发现 bias 还不够，要抓住它独有的结构。”
- “能不能从 uncertainty 本身出发，而不是做朴素补丁？”

## 高阶玩法

这个 radar 还会把 uncertainty 与其他题缝合：

- judge bias
- personality-conditioned judging
- RL exploration
- risk control
- structure-aware data selection
- evidential modeling

## 最终评价

这是一个很有“研究品味”味道的 skill。  
它不满足于把 uncertainty 当按钮用。  
它想知道这按钮内部是不是接错线了。
