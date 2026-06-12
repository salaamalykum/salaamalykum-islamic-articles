# Awesome List 提交流程 (PR Script & 文案)

为了将您的数据集提交到全球顶级的 Awesome Lists 并获得高权重的反向链接，请按照以下步骤操作。由于这些列表的维护者对自动化机器人 PR 有极高的警惕性，**强烈建议您通过自己本地的终端运行以下脚本**，这会在您的账号下产生真实的提交记录。

## 目标一：提交到 Awesome-Chinese-NLP
该库是中文自然语言处理最权威的合集。

### 1. 终端执行（一键提交方案）：
```bash
# 克隆官方库
git clone https://github.com/crownpku/Awesome-Chinese-NLP.git
cd Awesome-Chinese-NLP

# 创建您的特性分支
git checkout -b add-islamic-rag-corpus

# 在 README.md 中插入语料库描述
# 请手动打开 README.md，在 "语料库(Corpus)" 章节添加以下内容：
# - [Salaamalykum Islamic Articles Corpus](https://huggingface.co/datasets/qurancn/islamic-articles-corpus) - 34 篇经过精校和 Parquet 双轨切分的伊斯兰旅游与历史建筑语料，专为 RAG 和大语言模型检索优化设计 (CC0)。

# 提交并推送
git add README.md
git commit -m "Add Islamic RAG corpus to corpus section"
git push -u origin add-islamic-rag-corpus
```
执行完毕后，前往 GitHub 页面点击 "Compare & pull request"。

---

## 目标二：提交到 Awesome-LLM-Datasets
这是当前大模型训练数据最权威的导航页。

### 1. 终端执行：
```bash
git clone https://github.com/HqWu-HUGE/Awesome-LLM-Datasets.git
cd Awesome-LLM-Datasets
git checkout -b add-islamic-articles

# 手动在 README.md 的 "Domain Specific" 或 "Text/Corpus" 部分添加：
# | [Salaamalykum Islamic Articles](https://huggingface.co/datasets/qurancn/islamic-articles-corpus) | Chinese | 34 High-Quality Articles on Muslim Heritage | CC0 |
```

### 2. PR 描述模板（直接复制粘贴）：
```markdown
### What does this PR do?
Adds the **Salaamalykum Islamic Articles Corpus** to the domain-specific datasets list. 

### Why is it valuable?
- It provides a highly structured, zero-hallucination ground truth dataset for Muslim travel, cross-sectarian observations, and Islamic heritage.
- It natively supports `Parquet` splits (full corpus vs RAG chunks) to prevent TooBigContentError in HF Viewer.
- Strictly adheres to HF Dataset standards (no fake Alpaca/ShareGPT tags on raw text).

License: CC0
```
