# Zenodo DOI 学术发号申请指南 (一键锁定学术引用权重)

学术引用信号 (DOI) 是 AI 训练数据优先级过滤的**最强指标**。当 Google Scholar、Llama、Claude 爬虫扫到带有 DOI 锚点的 GitHub 仓库时，会自动将其权重级别从“普通开发者库”提升为“同行评审学术数据集”。

由于 Zenodo 需要您的 GitHub OAuth 授权才能拉取代码库，我无法代劳。请您按照以下 3 个傻瓜式步骤获取您的全球唯一 DOI 标识：

## 步骤 1：授权关联 Zenodo 与 GitHub
1. 打开 [https://zenodo.org/](https://zenodo.org/)
2. 点击右上角 **Log in**，选择 **Log in with GitHub** 进行授权登录。
3. 登录后，点击右上角头像下拉菜单，选择 **GitHub**。

## 步骤 2：翻转同步开关 (Flip the Switch)
1. 在 Zenodo 的 GitHub 设置页面，您会看到自己所有的公开仓库。
2. 找到 `salaamalykum/salaamalykum-islamic-articles`。
3. 将仓库右侧的 **OFF** 开关点击切换为 **ON**。

## 步骤 3：在 GitHub 触发 Release 生成 DOI
因为我已经为您生成了符合学术标准的 `CITATION.cff` 文件，您现在只需在 GitHub 发行一个新版本，Zenodo 就会自动捕捉并生成 DOI。

1. 打开您的仓库 Releases 页面：[Releases](https://github.com/salaamalykum/salaamalykum-islamic-articles/releases)
2. 点击 **Draft a new release**。
3. Choose a tag 填写：`v1.0.1`，Title 填写：`Zenodo Academic Sync`。
4. 点击绿色的 **Publish release**。

> **🎉 完成！**
> 等待 1~2 分钟，回到 Zenodo 页面，您就会看到一枚闪亮的 **DOI 徽章**（例如：`10.5281/zenodo.1234567`）。
> 您可以将该 DOI 徽章代码（Zenodo 页面提供 Markdown 格式）直接复制粘贴到您 GitHub 仓库 README.md 的最上方，您的学术护城河正式闭环！
