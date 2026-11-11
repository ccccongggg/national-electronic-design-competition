# TI 杯全国大学生电子设计竞赛 · 山东赛区归档

> 2026 TI 杯全国大学生电子设计竞赛 · 山东赛区参赛资料。
> 赛题相关结构：管内小球平衡装置、平衡小车（一号）、搬运小车（二号）、云台、MaixCAM 支架。

## 📸 现场素材

| 赛区现场 | 作品封箱记录 |
|---|---|
| [2026-TI杯山东赛区现场.jpg](media/event/2026-TI杯山东赛区现场.jpg) | [参赛作品封箱记录.jpg](media/process/参赛作品封箱记录.jpg) |

## 🧰 技术栈

TI **MSPM0G3507** + TI MSPM0 SDK + Code Composer Studio（CCS）+ 嘉立创 EDA 专业版 + SolidWorks。

## 📂 归档内容

| 目录 | 内容 |
| --- | --- |
| `software/competition-project/` | CCS 工程：BEEP、HWT101 陀螺仪、LED、MOTOR、MSPEED 测速、MYUART、OLED（字库 + 软件 IIC）、PID、Steering_gear 舵机、TIMER、TRACE 循迹等驱动 `.c/.h`，`empty.syscfg`、`targetConfigs/MSPM0G3507.ccxml`；另有电赛全能板 `.epro` |
| `hardware/competition-hardware/` | 25 电赛全能板 Plus 款（PCB 源文件 + 物料清单 + 问题说明 + 截图）、`M0母板/`（M03507 母板 `.epro2` + ReuseBlock）、`STM母版/STM扩展板.epro2`、机械结构 SolidWorks（小球管内平衡装置整机、一号 / 二号小车、云台、520 电机、齿轮齿条、开源结构 STL） |
| `media/event/`、`media/process/` | 封箱记录、赛区现场照片 |

## 🚀 打开工程

1. 安装 CCS + 匹配版本 MSPM0 SDK；
2. 导入 `software/competition-project/m0拓展板资料/单转弯可用/`；
3. 检查 SDK 路径 / 目标芯片 / 编译器 / 调试器配置；
4. 嘉立创 EDA 打开 PCB；SolidWorks 打开装配体时保留原目录结构。

## 🧹 清理说明

原始资料中的 IDE、烧录工具安装包、编译缓存、重复工程和通用厂商 SDK 未上传（TI MSPM0 SDK 含厂商测试私钥，应从 TI 官方渠道安装）。

## ⚠️ LFS 说明

PCB、CAD、图片等大文件由 **Git LFS** 托管；本地克隆需先安装 `git-lfs` 再 `git lfs pull`。
