# FiveAges Gen2 Robot USDs

中科第五纪（FiveAges）**第二代**机器人的 USD 仿真资产（[fiveages-gen2-robot-usds](https://github.com/fiveages-sim/fiveages-gen2-robot-usds)），作为 [robot_usds](https://github.com/fiveages-sim/robot_usds) 的子模块挂载于 `humanoid/FiveAges/Gen2/`。

## 目录结构

| 路径 | 说明 |
|------|------|
| `W2/` | FiveAges W2 折叠腰轮式人形 |
| `S2/` | FiveAges S2 立柱人形 |
| `components/Head_V1/` | 头部组件 |
| `components/Torso/` | 躯干组件（含身体 orbbec Sensor） |

## 克隆

本仓库通常不作为独立项目使用，请通过父仓库初始化子模块：

```bash
git clone git@github.com:fiveages-sim/robot_usds.git
cd robot_usds
git submodule update --init humanoid/FiveAges/Gen2
```

## 依赖

`W2` / `S2` 通过相对路径引用 `robot_usds` 主仓库中的以下资产：

- `manipulators/Tianji/M6_CCS/`
- `manipulators/Tianji/M20S_CCS/`
- `manipulators/Rokae/AR5_CCS_V2/`
- `manipulators/Fairino/ART7/`
- `sensors/`

`W2` 额外引用：

- `mobile_base/Linkhou/S2_V1/`
- `mobile_base/Linkhou/S2_V2/`
