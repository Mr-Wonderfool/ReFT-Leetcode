# ReFT-LeetCode

> Lab [at] Tongji University



### 流程

- 整理 leetcode 题目数据集
  - 已有
- 整理 prompt 模板，调用大模型 API，获得初步数据集
- 人类对数据集微调
  - 调整一下思维链
- 调大模型 API 生成代码，调用 leetcode API 生成评估结果，评价正确/错误
- 人类微调 + 自动校验





### 分工

- xzm: 读代码 + 搭建架构
- xrh: 初步数据集
- tkw: 人类微调数据集
- dza: 整理 leetcode API，方便评估代码是否正确