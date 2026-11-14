# DisGRem 项目工作说明

本仓职责：软件发布。当前状态见[STATE.md](STATE.md)，用法与技术背景见[README.md](README.md)。
在本工作区中，同时遵循[工作区说明](../../AGENTS.md)、[类别说明](../AGENTS.md)；需要命名、路径、版本或存储细节时查[公共规范](../../research_harness/policies/project_management.md)。独立克隆缺少这些外部文件时，以下项目事实和必要约定仍适用。

## 科研方式

探索优先。主动提出、推导、实现、比较和修正值得研究的想法，不能因为尚未证明或一次失败就提前放弃。必要时再依据证据、资源或当前目标缩小范围。使用标准数学语言和清楚自然的中文；正式结论准确说明依据，不编造证明、引用或实验。
旧总路由、旧L0/L1、旧强制科研Skill和旧阶段执行指令不再作为现行流程。历史文件保留事实；已有工具按具体任务选用。

## 项目特定条件

保留图连通性、光滑性、共识条件与理论/截断实现区别。既有run manifest和freeze contract继续维护来源记录。

## 实际入口

- [codes/main.py](codes/main.py)
- [codes/solvers/disgrem](codes/solvers/disgrem)

## 检查与运行

只读定位先查看相关文件与Git状态。按源码改动选择现有测试；freeze检查拒绝dirty/source mismatch，不默认重新发布。
简单改字只核对相应内容，改图优先复用原始数据。数学推导检查实际证明责任；代码改动选择受影响测试，探索实验按当前科学问题组织。

## 命名、保存与边界

名称表达科学含义和实际动作；按Python、MATLAB、Julia、C++各自惯例维护。已定义数学短符号和兼容API保留。清理路径或名称须同步调用、导入、配置和文档，不做跨文件盲替换。
当前状态只在指定入口更新；证明、原始结果、分析图表和历史各有来源，入口链接而不重复维护。新运行记录执行源码、实际配置和输出目录；已有等价记录优先复用。
本仓是独立保存边界；保护现有未提交工作、原始结果和冻结资产，不默认提交或推送。非Git原型按本地文件保存，不据此创建远端。

## 主源与交付职责

研究主源已完整归并至Research/disgrem；本仓保留交付及历史复现材料。持续修改先进入研究主源，历史Git与冻结文件保持。

交付仓自己的状态文件只记录构建和交付事实；研究状态与科研日志沿用研究主源的指定入口。导出记录源码版本或内容摘要、未提交修改、输入数据标识、文件清单与验证结果。目录名和本条约定不构成发布授权。

<!-- project-ownership -->
```json
{"maintenance": "delivery", "project_id": "disgrem", "source_root": "Research/disgrem", "status": "aligned"}
```
<!-- /project-ownership -->

<!-- unified-project-layout -->
## 统一目录职责

遵循[三类目录统一规范](../../research_harness/policies/research_delivery_layout.md)；本仓实际职责和路径映射见[project_layout.json](project_layout.json)。研究状态与交付状态分别维护。导出必须比对独有修改、记录来源散列并独立验证；迁移完成前保持真实待归并状态。独立克隆缺少工作区规范时，继续遵循本文件已有的主源、资产保护及验证要求。
<!-- /unified-project-layout -->

<!-- manuscript-review-delivery -->
## 文件组织与论文审阅交付

- 文件归属和目标命名遵循[详细目录](../../research_harness/policies/project_file_catalog.md)。算法、实验、输入、原始运行、分析和精简数据各归其指定位置；现有路径迁移前保持真实映射，保留历史资产。
- 论文按版本独立保存完整依赖，正文以章节组织；每轮论文交付从同版主源自动生成PDF、完整单文件review.tex、review.zip和source.zip，写入该版output，索引记录实际位置。
- 单文件包含正文、附录、宏定义、图注、表格和实际文献条目；保留TeX语义，图件及样式随审阅包提供。生成稿不独立编辑，外部意见回写主源后重新生成。
- 交付前核对内容与引用，并在隔离目录编译审阅包；记录源版本、格式、输入输出摘要、命令和实际验证结果。未生成或未验证的产物明确列为待完成。日常编辑不逐次打包，规则维护不触发论文改版。
- 完整要求见[审阅交付规则](../../research_harness/policies/manuscript_review_delivery.md)。Publish只接收确定副本，Public保持软件职责；独立克隆缺少工作区规则时仍执行本节摘要。交付回复链接PDF和review.tex，按需链接两个压缩包。
<!-- /manuscript-review-delivery -->
