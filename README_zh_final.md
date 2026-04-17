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

## 逐节质量标注（发布前检查）

说明：以下状态用于发布前把控质量。
- **已翻译**：英文正文已替换为中文，结构完整。
- **已润色**：术语、语气与标点已做统一优化。
- **建议人工复核**：建议由你做最终语义把关（重点核对学术措辞是否符合你偏好的表达风格）。

| 章节 | 状态 | 备注 |
|---|---|---|
| 摘要（Abstract） | 已翻译 / 已润色 | 建议人工复核数值表述语气 |
| 引言（Introduction） | 已翻译 / 已润色 | 建议人工复核领域术语偏好 |
| 问题定义（Problem Definition） | 已翻译 / 已润色 | 公式已保留原式，建议复核术语细微差异 |
| 相关工作（Related Work） | 已翻译 / 已润色 | 建议复核文献叙述语气 |
| 预备知识（Preliminaries） | 已翻译 / 已润色 | 引理与证明文字已中文化 |
| Shannon 下界（SLB） | 已翻译 / 已润色 | 证明结构与公式完整保留 |
| QJL 小节 | 已翻译 / 已润色 | 定义、引理、证明均已中文化 |
| TurboQuant：MSE 章节 | 已翻译 / 已润色 | 算法与定理环境完整，建议复核算法文字风格 |
| TurboQuant：内积章节 | 已翻译 / 已润色 | 定理与证明中文化完成 |
| 下界（Lower Bounds） | 已翻译 / 已润色 | 关键论证完整保留 |
| 实验（Experiments） | 已翻译 / 已润色 | 图表、数据、结论已保留并中文化 |
| 附录术语表 | 已新增 / 已润色 | 可按团队术语规范继续扩展 |

## 建议的最终人工复核清单（10 分钟版）

- [ ] 通读摘要与结论：确认措辞是否符合你对论文“口吻”的要求。  
- [ ] 抽查 3 个定理（MSE、内积、下界）：确认叙述与原意一致。  
- [ ] 抽查 3 个图注与 1 个表注：确认中英文术语完全统一。  
- [ ] 编译一次并翻阅 PDF：确认分页、公式、图表显示符合预期。  

