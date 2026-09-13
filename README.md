# GEO Analysis: GSE42872

## 项目背景
分析 Vemurafenib 处理黑色素瘤细胞（A375）后的基因表达变化。

## 数据来源
GEO 数据集：GSE42872（平台 GPL6244）

## 分析方法
- **语言**：Python (GEOparse, pandas, scipy, gseapy)
- **核心步骤**：探针注释 → 差异表达分析（t-test + FDR校正） → 火山图、热图 → KEGG 富集分析

## 主要结果
- 筛选出 **1123 个**显著差异基因（|log2FC| > 1，P < 0.05）
- KEGG 富集揭示 Vemurafenib 作用机制：**Cell cycle**、**DNA replication**、**p53 signaling** 等通路显著富集

## 文件说明
- `geo_analysis.ipynb`：完整分析代码
- `volcano_plot.png`：火山图
- `heatmap.png`：热图
- `significant_genes.csv`：显著基因列表
