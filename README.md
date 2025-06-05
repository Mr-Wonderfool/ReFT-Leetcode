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

### 一些可能用到的资料
- [Huggingface上的Leetcode数据集](https://huggingface.co/datasets/newfacade/LeetCodeDataset)，含有问题、题目框架代码、测试用例和测试代码，同时给出了模型正确的输出，[配套的论文](https://arxiv.org/abs/2504.14655)

### 各自的任务梳理
- XZM(6.5): 
  * [ ] 给出数据集需要的格式，可以参考gsm8k，确定要用P-CoT还是N-CoT
  * [x] 模型选择为`hf_models/CodeLlama-7b-hf`，tokenizer对应选择为`hf_models/CodeLlama-7b-hf`
  * [ ] 给出环境依赖方便远程环境重建
  * [ ] 参照ReFT给出项目初步架构，在gsm8k上运行成功