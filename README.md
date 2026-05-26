# 实证报告包说明

本仓库包含一份基于数据文件 `数据.dta` 的中文实证报告。报告主题为：智能化转型、过度教育与企业就业结构。

## 目录

- `report/main.tex`：LaTeX 源文件
- `report/main.pdf`：已编译 PDF
- `report/tables/`：LaTeX 表格文件
- `report/figures/`：图表 PDF/PNG
- `results/`：描述性统计、回归结果、变量字典 CSV
- `code/build_empirical_report.py`：完整复现脚本
- `PLAN.md`：执行计划

## 复现方式

将原始 `数据.dta` 放在脚本中指定路径，或修改脚本开头的 `RAW` 变量后运行：

```bash
python code/build_empirical_report.py
```

脚本依赖：pandas、numpy、matplotlib、linearmodels、pyhdfe。

## 注意

1. 原始数据文件 `数据.dta` 未上传到本仓库；如需完全离线复现，请将原始数据放入相应目录。
2. 报告依据变量名和上传参考文献识别变量含义；若后续有正式数据说明书，应据此校正变量解释。
3. 报告为课程/研究训练型实证报告，不声称达到期刊投稿的完整原创性要求。
