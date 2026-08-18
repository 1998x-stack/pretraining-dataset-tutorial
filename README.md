# 📦 LLM预训练数据集 · 从入门到精通

> 📘 28章 实战体系 · 交互式 HTML 课程

> **English TL;DR:** An all-Chinese 28-chapter course on **LLM pretraining datasets** — the data that sets a model's ceiling (GIGO, Scaling Law / Chinchilla, dosage). Surveys the base corpora (RedPajama-1T, SlimPajama, Dolma, Chinese SkyPile-150B / WuDao / CLUECorpus, vertical: The Stack, OpenWebMath/ProofPile, arXiv, FLAN) and Common Crawl (WARC/WET, FineWeb's 95% reduction). The engineering core: license compliance & PII redaction, mixing philosophy (70-15-10-5 / curriculum), acquisition & format parsing (warcio, trafilatura), language detection, exact (SHA-1, suffix-array) & fuzzy (MinHash+LSH, embeddings) dedup, model-based quality scoring (FineWeb-Edu, DCLM), harmful-content filtering, distributed processing (MapReduce/Slurm/Ray), streaming (HuggingFace Datasets / WebDataset), benchmark contamination, data versioning (DVC) & provenance, synthetic data (FineWave, model collapse), multilingual/low-resource, curriculum & dynamic scheduling, code/math handling, and toolchains (DataTrove, NeMo Curator w/ GPU acceleration). Ends with 2026 trends (Densing Law, AI-native data factories), a 1B-model dataset capstone, and TB→PB scaling.

## 📖 课程简介

本课程围绕 **LLM 预训练数据**做系统性工程讲解：先是数据决定模型上限的认知与全球基座语料全景（开源复现、中文语料、垂直领域），再深入 Common Crawl 与 WARC 解析；重点讲解一套生产级清洗管线——语言识别、多级去重（精确/MinHash/语义）、基于模型的评分（FineWeb-Edu/DCLM）、有害内容过滤、分布式处理与流式加载。随后覆盖污染检测、数据版本与溯源、合成数据、多语言、课程学习、代码/数学专项，以及 DataTrove / NeMo Curator（GPU 加速）两大工具链，最后以「为 1B 模型构建训练集」的端到端实战与 PB 级规模化收束。

## 🚀 快速开始

```bash
open index.html   # macOS，纯静态即开即看
```

## 📂 项目结构

```text
pretraining-dataset-tutorial/
├── index.html / 01.html ~ 28.html / courses.json / theme.css
```

## 📖 章节分段

| 阶段 | 章节 | 核心 |
|------|------|------|
| **认知与语料全景** | 01–05 | 数据上限、开源/中文/垂直语料、Common Crawl |
| **合规与配比** | 06–07 | 许可合规、数据配比策略 |
| **清洗管线** | 08–14 | 采集解析、语言识别、精确/模糊/语义去重、模型评分、有害过滤 |
| **分布式与工程** | 15–18 | 分布式处理、流式加载、污染检测、版本与溯源 |
| **增强与专项** | 19–22 | 合成数据、多语言、课程规划、代码/数学 |
| **工具链与规模化** | 23–28 | DataTrove / NeMo Curator、质量评估、2026 前沿、1B 实战、PB 级 |

## ✨ 亮点

- 数据清洗「采集→去重→评分→过滤→工具链」全线闭环
- 中文语料 + 许可证/PII + 防污染全覆盖
- 含 DataTrove / NeMo Curator（GPU 加速）两大工具链与 1B 数据集实战

## 🎯 前置知识

- 适合：预训练数据工程师 / LLM 训练团队
- 建议具备：Python + 大数据/分布式基础概念

## ✨ 特色

- 以 GIGO 认知贯穿，理论 + 工程 + 规模化三位一体
- 即开即用纯静态 HTML

---
*本课程由 `pretraining-dataset-tutorial/` 项目维护。*