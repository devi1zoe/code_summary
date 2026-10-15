# SABCS: Sparse Attention-Based Code Summarization

面向长代码摘要生成的结构感知稀疏注意力研究。模型结合 Global-local、Top-k 注意力以及基于抽象语法树（AST）和控制流图（CFG）的结构信息，旨在减少注意力冗余并建模长距离代码依赖。

**[阅读论文 PDF](paper/sabcs.pdf)** · [BibTeX 引用](paper/citation.bib) · [相关专利申请](#相关专利申请)

## 论文信息与版本状态

- 标题：*SABCS: Sparse Attention-Based Code Summarization*
- 作者：Qing Mi、Yufan Han、Guoxiang Jiang。
- 文稿标注 Yufan Han 与 Guoxiang Jiang 为同等贡献，Qing Mi 为通讯作者。
- 单位：Beijing University of Technology（北京工业大学）。
- **当前上传版本为草稿**：PDF 仍包含会议模板、DOI、部分实验数值及引用占位符，不能据此认定已正式发表。引用条目按未发表文稿记录，不填写虚构会议或 DOI。

## 相关专利申请

本研究相关成果已申请中国发明专利，申请公开信息如下：

- **名称（公开索引英文题名）**：*Long code abstract generation method based on structure-guided sparse attention mechanism*。
- **申请人**：北京工业大学（Beijing University of Technology）。
- **发明人（按公开索引顺序）**：Qing Mi、Guoxiang Jiang、Yufan Han。
- **申请号**：`202511202527.7`。
- **申请公开号**：`CN121029230A`。
- **申请日 / 申请公布日**：2025-08-26 / 2025-11-28。
- **公开查询**：[专利申请公开信息（Patsnap）](https://eureka.patsnap.com/patent/CN121029230A) · [发明人及申请信息（韩国国家知识平台）](https://k-knowledge.kr/srch/read.jsp?id=281284475)。

本节记录的是专利申请公开信息；所附 SABCS 论文仍为未发表草稿。

## 方法概要

1. 使用 Global-local 注意力兼顾局部上下文和长距离信息。
2. 使用 Top-k 注意力筛选重点关注的位置。
3. 将 AST 与 CFG 的结构信息组织为 Logic Graph，并设计结构感知注意力规则。

文稿讨论超过 1,024 tokens 的长代码，涉及 CodeXGLUE 子集和 Hu 等人的数据集，以 BLEU-4、METEOR、ROUGE-L 评价摘要质量。由于当前稿件仍有未完成的结果占位符，本仓库不将摘要中的性能描述作为可复核的最终结论。

## 仓库内容

```text
.
├── README.md
├── LICENSE
└── paper/
    ├── sabcs.pdf       # 作者提供的论文草稿，原文件保留
    └── citation.bib    # 未发表文稿的引用信息
```

当前仓库用于论文存档，尚未上传模型实现、训练脚本、数据处理流程、权重与实验记录，因此暂不提供可运行的复现命令。

## 后续待补材料

- 完成占位符校对的最终论文版本，以及确认后的出版信息（如有）。
- 数据划分与长代码筛选规则、运行依赖、模型及训练入口。
- 完整指标、基线比较、消融结果和对应实验配置。

## Citation

使用本草稿时，请注明版本状态。可复制 [paper/citation.bib](paper/citation.bib) 中的条目；正式发表后应更新为对应出版信息。
