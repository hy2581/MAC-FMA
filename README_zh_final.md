# 中文版论文交付清单（TurboQuant）

本仓库当前已提供可直接编译的完整中文版论文源文件与 PDF 产物。

## 主要文件

- `main_zh_full.tex`：完整结构中文版 TeX（保留原论文公式、图表、定理、算法、引用与编号体系）
- `main_zh_full.pdf`：由 `main_zh_full.tex` 编译得到的中文版 PDF

## 编译方式

建议使用 XeLaTeX：

```bash
xelatex -interaction=nonstopmode -halt-on-error main_zh_full.tex
bibtex main_zh_full
xelatex -interaction=nonstopmode -halt-on-error main_zh_full.tex
xelatex -interaction=nonstopmode -halt-on-error main_zh_full.tex
```

## 一致性状态

- [x] 公式与编号保留
- [x] 图表与路径保留
- [x] 算法、定理、证明环境保留
- [x] 参考文献流程（BibTeX）可用
- [x] 正文中文化并完成术语统一
- [x] 附录新增中英文术语对照表

## 术语统一约定（摘要）

- bit-width / bits：位宽
- embedding：嵌入
- inner-product error：内积误差
- recall：召回率
- Full-Precision：全精度

