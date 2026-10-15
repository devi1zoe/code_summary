# SABCS: Sparse Attention-Based Code Summarization

面向长代码摘要生成的结构感知稀疏注意力研究。项目探索将抽象语法树
（AST）与控制流图（CFG）中的结构信息引入注意力机制，以建模代码中的
长距离依赖，减少无关信息对摘要生成的干扰。

本仓库收录项目研究文稿及相关专利申请信息。

[研究文稿（PDF）](paper/sabcs.pdf) · [相关专利申请](#相关专利申请)

## 研究内容

- 结合 Global-local 与 Top-k 注意力，关注局部上下文和关键代码位置。
- 融合 AST 与 CFG，构建代码逻辑图（Logic Graph）。
- 根据代码中的序列距离与图结构关系，设计结构感知注意力规则。

## 研究文稿

**SABCS: Sparse Attention-Based Code Summarization**

- 作者：Qing Mi、Yufan Han、Guoxiang Jiang。
- 单位：北京工业大学。
- Yufan Han 与 Guoxiang Jiang 为同等贡献，Qing Mi 为通讯作者。
- 文稿状态：未发表。

[阅读研究文稿](paper/sabcs.pdf) · [BibTeX](paper/citation.bib)

## 相关专利申请

本项目相关技术已形成中国发明专利申请，并已公开。

- **名称**：Long code abstract generation method based on structure-guided sparse attention mechanism
- **申请人**：北京工业大学。
- **发明人**：Qing Mi、Guoxiang Jiang、Yufan Han。
- **申请号**：202511202527.7。
- **申请公开号**：CN121029230A。
- **申请日**：2025-08-26。
- **申请公布日**：2025-11-28。

[查看专利公开信息](https://eureka.patsnap.com/patent/CN121029230A)

## 仓库内容

- `paper/sabcs.pdf`：研究文稿。
- `paper/citation.bib`：文稿引用信息。

本仓库保存研究文稿、引用信息及相关专利申请资料。
