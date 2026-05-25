# DABIC Gravity Vinton 任务附录包

本目录为 SE-Bench 任务 `dabic_gravity_vinton` 的提交附录材料，按任务发布、运行环境、评分器、评测记录和说明文档组织。

目录结构：

```text
agent-start/    agent 起始材料，包括论文、Vinton 数据、starter 脚本和任务 README
baseline/       本次 30min/2h 有效 run 的 run_history 与 v3.4 复评日志
docs/           评分方案、地球物理评价方案、复评说明和分数曲线
environment/    Dockerfile 与 requirements
scorer/         当前正式评分脚本和 score.sh
tasks/          SE-Bench 任务 JSON
```

当前正式评分版本：

```text
v3.4 = BALANCED_C_V3.4 + STRUCTURAL_PENALTY_V3.4
```

当前正式评分文件 SHA256：

```text
ded45a140d3658f146ca2911a4173e00ac0dc9602f00baa08950a37cda42ee34
```

当前校准结果：

```text
30min = 14.9146
2h    = 27.5152
```

说明：当前 hidden 场景逻辑已经内嵌在 `scorer/evaluate.py` 中，不再使用单独的 `hidden_scenarios_v2.py` 文件。
