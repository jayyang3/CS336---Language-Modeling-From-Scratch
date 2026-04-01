# CS336: 从零开始的语言建模 (Language Modeling From Scratch)

## 📖 项目概述

这是一个用于学习斯坦福大学CS336课程的学习仓库。该课程重点介绍如何从基础原理出发，从零开始构建大型语言模型(LLMs)。

## 🎯 学习目标

本仓库的目标是深入理解和实践以下核心概念：

- **Transformer架构**：自注意力机制、多头注意力、位置编码
- **训练基础**：数据预处理、损失函数、优化算法
- **语言建模**：预训练、微调、提示工程
- **评估与推断**：模型评估、文本生成、性能优化
- **实践应用**：从头构建小型LLM并进行训练

## 📁 仓库结构

```
CS336---Language-Modeling-From-Scratch/
├── README.md                 # 本文件
├── LICENSE                   # 项目许可
├── notebooks/                # Jupyter笔记本（作业和教程）
├── code/                      # Python实现代码
│   ├── models/              # 模型实现
│   ├── data/                # 数据处理
│   └── utils/               # 工具函数
├── assignments/             # 课程作业
├── resources/               # 学习资源和参考资料
└── outputs/                 # 训练结果和检查点
```

## 🚀 快速开始

### 环境要求

- Python 3.10+
- [uv](https://github.com/astral-sh/uv) - 快速的Python包管理器
- 可选：CUDA/ROCm（GPU加速）

### 安装

#### 1. 安装 uv

```bash
# macOS / Linux
curl -LsSf https://astral.sh/uv/install.sh | sh

# Windows (使用 PowerShell)
powershell -c "irm https://astral.sh/uv/install.ps1 | iex"

# 或使用包管理器
pip install uv
```

#### 2. 克隆并设置项目

```bash
# 克隆仓库
git clone https://github.com/yourusername/CS336---Language-Modeling-From-Scratch.git
cd CS336---Language-Modeling-From-Scratch

# uv 会自动创建虚拟环境并安装依赖
uv sync

# 激活虚拟环境
source .venv/bin/activate  # Linux/Mac
# 或
.venv\Scripts\activate  # Windows
```

#### 3. 可选：安装额外依赖

```bash
# 安装开发工具（linting, testing）
uv sync --extra dev

# 安装 JAX 支持（如果需要）
uv sync --extra jax

# 安装 TensorBoard 支持
uv sync --extra tensorboard
```

## 📚 课程大纲

| 周次 | 主题 | 关键概念 | 作业 |
|-----|------|--------|------|
| 1 | 基础知识回顾 | 神经网络基础、反向传播 | HW1 |
| 2 | Transformer基础 | 自注意力、多头注意力 | HW2 |
| 3 | 语言建模预训练 | 下一词预测、序列建模 | HW3 |
| 4 | 微调与适配 | 指令微调、LoRA | HW4 |
| 5 | 评估与生成 | 困惑度、束搜索、温度采样 | HW5 |

## 💡 学习建议

1. **按顺序学习**：从基础概念开始，逐步理解高级主题
2. **理论与实践结合**：阅读论文同时实现代码
3. **动手编码**：不只是阅读，要亲自实现关键算法
4. **调试和实验**：尝试修改超参数，观察模型行为
5. **记录笔记**：在学习过程中记录重点和疑问

## 📖 推荐资源

### 论文
- [Attention Is All You Need](https://arxiv.org/abs/1706.03762) - Transformer架构
- [BERT: Pre-training of Deep Bidirectional Transformers](https://arxiv.org/abs/1810.04805)
- [Language Models are Unsupervised Multitask Learners](https://d4mucfpksywv.cloudfront.net/better-language-models/language_models_are_unsupervised_multitask_learners.pdf) - GPT-2

### 书籍与教程
- [Deep Learning with PyTorch](https://pytorch.org/) - 官方文档
- [The Transformer Model Explained](https://medium.com/)
- Stanford CS236N 笔记

### 数据集
- WikiText
- GLUE
- Common Crawl

## 🛠️ 技术栈

- **包管理**: uv - 快速的Python包和项目管理
- **深度学习框架**: PyTorch (或 JAX)
- **数据处理**: Hugging Face Datasets
- **模型**: Hugging Face Transformers
- **可视化**: TensorBoard, Matplotlib
- **开发工具**: Jupyter, Black, Ruff, MyType
- **版本控制**: Git

## 📝 作业提交

- 将完成的作业保存在 `assignments/` 文件夹
- 在相应的README中记录实验结果
- 使用清晰的代码注释和文档

## ❓ 常见问题

**Q: 我没有GPU怎么办？**
A: 可以使用CPU进行学习和调试，但训练较大模型时会很慢。考虑使用云服务(Google Colab, HuggingFace Spaces)。

**Q: 需要什么背景知识？**
A: 需要基本的Python编程、线性代数和微积分知识。

**Q: 如何贡献改进？**
A: 欢迎提出Issue和Pull Request来改进代码和文档。

## 📧 联系与反馈

- 如有问题，请提交Issue
- 欢迎任何建议和改进

## 📄 许可

本项目基于 [LICENSE](LICENSE) 中指定的许可协议发布。

---

## 🌟 致谢

感谢斯坦福大学和CS336课程团队提供的优质教学资源。

**最后更新**: 2026年4月
