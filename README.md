# LLM 学习笔记

大语言模型（LLM）相关学习资料整理，使用 [Obsidian](https://obsidian.md/) 编写，通过 [Quartz](https://quartz.jzhao.xyz/) 发布为静态网站。

## 🌐 在线阅读

👉 **[reggiws.github.io/llm-notes](https://reggiws.github.io/llm-notes/)**

## 📂 目录

| 目录 | 内容 |
|------|------|
| [数学与概念](数学与概念/) | KL 散度、香农熵、LoRA、TV 散度 |
| [模型训练](模型训练/) | 激活函数、优化器、分布式训练、混合精度训练、显存计算 |
| [手撕代码](手撕代码/) | Attention 等核心机制的手动实现 |
| [模型可解释性](模型可解释性/) | 模型可解释性推理方法 |

## 🛠 技术栈

- **笔记编写**：[Obsidian](https://obsidian.md/)
- **静态站点**：[Quartz 5](https://quartz.jzhao.xyz/)
- **部署**：[GitHub Pages](https://pages.github.com/) + GitHub Actions

## 📝 本地运行

```bash
git clone https://github.com/Reggiws/llm-notes.git
cd llm-notes
npm ci
npx quartz plugin install --from-config
npx quartz build -d . --serve
```

然后访问 `http://localhost:8080`。

## 📄 License

[CC BY 4.0](LICENSE)
