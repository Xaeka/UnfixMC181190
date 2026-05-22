# Unfix MC-181190

[中文](#chinese) | [English](#english)

---

## 中文

### 简介

此模组恢复了治愈村民折扣叠加的功能，该功能在 1.20.2 的首个快照 **23w31a** 中被 Mojang "修复"（即 [MC-181190](https://bugs.mojang.com/browse/MC-181190)）。

在原版 1.20.2+ 中，多次治愈同一个僵尸村民不会让交易价格进一步降低。本模组将此机制的数值恢复为 23w31a 之前的行为，使折扣可以重新叠加。

### 关于此移植版

本版本是 [asablock 的原始 Fabric 模组](https://github.com/asablock/unfixmc181190) 的非官方 **NeoForge 移植版**，由 **Xaeka** 移植。

| 项目 | 信息 |
|------|------|
| 原始作者 | [asablock](https://github.com/asablock) |
| 移植作者 | [Xaeka](https://github.com/Xaeka) |
| 适用平台 | **NeoForge** |
| 适用游戏版本 | **Minecraft 1.21.11**（群骑与纷争 / Mounts of Mayhem） |
| NeoForge 版本 | 21.11.42+ |
| 模组版本 | 1.0.2 |
| 源代码 | [GitHub](https://github.com/Xaeka/UnfixMC181190/tree/1.21.11-NeoForge) |

### 技术说明

本模组通过 Mixin 修改 `net.minecraft.world.entity.ai.gossip.GossipType` 枚举的静态初始化常量，将 Mojang 在 23w31a 中下调的 `maxValue` 和 `shareDecrement` 恢复为原始数值，从而还原治愈村民折扣可叠加的机制。

### 许可证

本模组沿用原始项目的 [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) 许可证。

---

## English

### Introduction

This mod brings back the feature of cured villager's discount stacking which was "fixed" by Mojang in the first 1.20.2 snapshot **23w31a** (see [MC-181190](https://bugs.mojang.com/browse/MC-181190)).

In vanilla 1.20.2+, curing the same zombie villager multiple times will not further reduce trading prices. This mod restores the pre-23w31a behavior, allowing discounts to stack again.

### About This Port

This is an unofficial **NeoForge port** of [asablock's original Fabric mod](https://github.com/asablock/unfixmc181190), ported by **Xaeka**.

| Item | Details |
|------|---------|
| Original Author | [asablock](https://github.com/asablock) |
| Port Author | [Xaeka](https://github.com/Xaeka) |
| Platform | **NeoForge** |
| Game Version | **Minecraft 1.21.11** (Mounts of Mayhem) |
| NeoForge Version | 21.11.42+ |
| Mod Version | 1.0.2 |
| Source Code | [GitHub](https://github.com/Xaeka/UnfixMC181190/tree/1.21.11-NeoForge) |

### Technical Details

This mod uses Mixin to modify the static initializer constants of the `net.minecraft.world.entity.ai.gossip.GossipType` enum, restoring the `maxValue` and `shareDecrement` values that Mojang lowered in 23w31a, thereby re-enabling the stacking of cured villager discounts.

### License

This mod inherits the original project's [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) license.
