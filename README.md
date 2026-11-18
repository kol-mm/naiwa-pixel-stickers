# 奶家族像素表情包

给《奶蛙的结合》和奶家族谱里的角色做微信动态表情。这套 Codex Skill 收录了角色定稿、动作范例和 GIF 检查脚本，适合做新表情，也适合拿已有动图回来改动作或查杂色。

| 奶猫踩奶 | 奶鼠递奶酪 |
| --- | --- |
| <img src="assets/cat-knead.gif" width="144" height="144" alt="奶猫前爪交替踩奶，动作自然循环"> | <img src="assets/mouse-share.gif" width="144" height="144" alt="奶鼠双爪把奶酪递出来，在伸到最远处停一下"> |

踩奶是一拍接一拍的动作，下一轮顺势接上。奶鼠递奶酪则在伸出手时停一下，让聊天里的人看清它在说「给你」。

## 做一枚表情

把整个仓库放在 Codex 的 `~/.codex/skills/naiwa-pixel-stickers/` 目录下。比如，想试做奶猫踩奶时，可以在新对话里输入下面这句话。

> 用 $naiwa-pixel-stickers 做一枚奶猫踩奶。眼睛慢慢眯起来，两只前爪轮流踩，发到聊天里也要看得清。

从角色定稿开始画，再按动作选择自然循环或在结尾停一拍。制作流程、可用原图和微信投稿尺寸都在仓库里。[制作流程](SKILL.md) · [角色定稿](references/models.md) · [动作与节奏](references/motion-quality.md) · [微信导出规格](references/wechat-delivery.md)

## 检查导出的 GIF

在仓库目录运行下面两行，就能用自带的奶猫样例试一次。检查脚本会核对 240 × 240 的画布、透明背景、循环和文件大小。把最后的路径换成自己的 GIF 即可。

```sh
python -m pip install Pillow
python scripts/check_gif.py assets/cat-knead.gif
```

## 开源许可

原创制作说明、脚本、工具配置及原创帧数据采用 MIT 许可，允许商用、修改、再分发和销售副本。复制或分发这些内容或其实质性部分时，须保留版权声明和许可全文。角色原图和示例动图各按自身授权使用，不属于这次 MIT 授权的范围。[完整协议](LICENSE) · [素材说明](assets/NOTICE.md)

本次变更不撤销此前版本已授予的 GPL-3.0-only 权利。

## 奶系桌面壁纸

要把同一批角色做成桌面动态壁纸，可以使用另一份 Skill。它收录了横幅取景、角色姿势还原和视频循环检查，并附数字博物馆的动态预览。[本仓库收录的版本](skills/naiwa-pixel-wallpapers) · [壁纸 Skill 仓库](https://github.com/kol-mm/naiwa-pixel-wallpapers)
