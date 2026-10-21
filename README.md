# 智能驾驶算法专家

面向智能驾驶算法全链路的专家：从 BEV / Occupancy 感知与多传感器融合，到预测决策规划控制、端到端智驾模型、数据闭环、车端部署与功能安全，用"指标 + 预算 + 边界条件"的方式把算法问题拆成可验证的量产方案。

## 类型

Agent 型（单个 AI 专家）

## 功能

- **感知**：BEV 检测、Occupancy 网络、时序融合、LiDAR/相机/毫米波融合、3D 跟踪与在线建图、在线标定与失效降级
- **预测与规控**：交互式轨迹预测、Lattice / EM / iLQR / MPC 规划、学习型规划、横纵向控制与舒适度约束
- **端到端**：UniAD / VAD 类范式、VLA 与世界模型路线、蒸馏与安全兜底、端到端与模块化混合架构取舍
- **数据与训练**：数据采集触发、自动标注、长尾挖掘、训练压缩与回归流水线
- **部署与安全**：Orin/Thor 算力与时延预算、TensorRT 量化优化、ODD / SOTIF / ISO 26262 分析
- **评价体系**：mAP/NDS、minADE/minFDE、MPI 接管里程、舒适度与碰撞口径

## 使用示例

- 帮我设计一套面向城市 NOA 的 BEV 感知方案：传感器配置、模型结构、数据需求和评价指标怎么定？
- 端到端智驾模型（UniAD / VAD 这类）和传统感知+规控模块化方案比，量产落地的取舍在哪？给我一张对比表。
- 要在单颗 Orin-X（254 TOPS）上跑 6V BEV 感知加规控，帮我把时延预算和量化部署策略排一遍。

## 头像

头像已自动生成在 `avatars/` 目录下。如需替换为自定义头像，要求：
- 格式：PNG（推荐）或 JPG
- 尺寸：512×512 px
- 大小：单张不超过 500KB

## 安装

将专家包目录放到专家目录下：

```
/Users/dzp/.workbuddy/plugins/marketplaces/my-experts/plugins/autonomous-driving-algorithm-expert/
```

然后运行注册命令使其可见：

```bash
python3 scripts/register_expert.py <expert-dir>
```

## 打包分享

```bash
python3 scripts/package_expert.py <expert-dir>
```
