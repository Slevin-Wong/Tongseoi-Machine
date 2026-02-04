# 阶段三：美学库重组（v2.0）- 第一部分：角色系统

---

## 📋 美学库结构说明

原指令集第2-6部分包含大量创意组件，总计约200行。这是整个系统的"素材库"。

**重组策略：**
1. **模块化拆分**：角色系统 + 服装系统 + 场景系统 + VIBE引擎
2. **标签化索引**：每个组件分配唯一标签，便于快速查找
3. **组合建议**：避免固定搭配，提供创新组合示例
4. **降低篇幅**：精简冗余描述，保留核心关键词

本文档覆盖：**第二部分 - 角色蓝图**（面部、身体、发型、妆容、纹身）

---

## 👤 第二部分：角色蓝图（Character Blueprint）

### 快速导航
- [2.1 面部系统](#21-面部系统) - 骨相、五官、种族选项
- [2.2 身体系统](#22-身体系统) - 体型、局部美学、皮肤质感
- [2.3 发型系统](#23-发型系统) - 发质、长度、造型、发色
- [2.4 妆容系统](#24-妆容系统) - 时尚前卫 vs 生活自然
- [2.5 纹身系统](#25-纹身系统) - 位置、风格、叙事功能

---

## 2.1 面部系统（Face System）

### 2.1.1 核心面部基底（默认）

**骨相基础：**
- 东亚美女骨相（East Asian beauty）
- 对称、女性化、精致的脸型
- small refined chin（小巧下巴）
- smooth jawline（流畅下颌线）

**四维美学融合（必选）：**

| 维度 | 关键词 | 说明 |
|-----|--------|------|
| **眼睛** | large expressive eyes, bright eyes, long voluminous eyelashes, double eyelids | 幼态与神采 |
| **鼻子** | high nasal bridge, small refined nose, delicate nose tip | 立体与精致 |
| **嘴唇** | full plump lips, rosy lips, soft and defined cupid's bow | 健康与性感 |
| **肤质** | pale porcelain skin, soft natural glow | 通透与气血感 |

---

### 2.1.2 个性化特征微调（可选）

**用途**：增加辨识度，避免审美疲劳

**眼部变体：**
- `[Face-Eye-01]` Phoenix eyes（丹凤眼）
- `[Face-Eye-02]` Light-colored iris（琥珀瞳/浅色瞳孔）
- `[Face-Eye-03]` Heterochromia（异色瞳）

**鼻部变体：**
- `[Face-Nose-01]` Aquiline nose（微驼峰鼻，增加英气）
- `[Face-Nose-02]` Upturned nose / button nose（小翘鼻，增加娇俏感）

---

### 2.1.3 种族选项（严格限制使用）

**⚠️ 重要说明**：以下选项违反"高度写实照片"基调，已移至🔴禁令

**已禁用：**
- ❌ elf ears（精灵耳）
- ❌ kemonomimi（兽耳：fox ears, cat ears, wolf ears）
- ❌ angel halo/wings（天使光环/翅膀）

**默认：**
- ✅ Human（人类）- 唯一允许选项

---

## 2.2 身体系统（Body System）

### 2.2.1 核心体型（默认优先级）

**基准描述：**
```
a slender, toned woman with a captivating, naturally curvaceous hourglass figure
（苗条、健美、自然曲线的沙漏形身材）
```

**腰腹细节（可选强化）：**
- slim, defined waistline（纤细分明的腰线）
- athletic obliques / v-cut abs（马甲线）

---

### 2.2.2 体型微调（根据角色气质）

**触发条件**：服务于特定角色设定或VIBE引擎

| 气质类型 | 体型调整 | 关键词 |
|---------|----------|--------|
| 果敢飒爽 | 运动感健美 | athletic physique, toned muscles, fit body |
| 清纯脱俗 | 纤细骨感 | slender delicate frame, petite build, graceful thinness |
| 性感魅惑 | 强调曲线 | voluptuous curves, feminine silhouette, shapely figure |

---

### 2.2.3 局部美学焦点（选择性强化）

**规则**：每个创意选择 **最多1项** 进行重点刻画，与姿态模块联动

**可选列表：**

| 标签 | 关键词 | 适配姿态 |
|------|--------|----------|
| `[Body-Neck]` | beautiful swan neck | 侧面、仰视角度 |
| `[Body-Collarbone]` | prominent collarbones | 露肩服装、前倾姿态 |
| `[Body-Back]` | well-defined elegant back | 背面、回眸姿态 |
| `[Body-Shoulder]` | sharp right-angle shoulders | 吊带、无袖服装 |
| `[Body-Abs]` | defined athletic abs | 运动风、露脐装 |
| `[Body-Waist]` | slim waistline | 束腰服装、侧身姿态 |
| `[Body-Hips]` | prominent peach hips | 紧身下装、背面姿态 |
| `[Body-Legs]` | long legs, toned leg lines | 短裙短裤、全身景 |

**使用示例：**
```
✅ "featuring prominent collarbones, wearing an off-shoulder gown"
❌ "featuring swan neck, collarbones, back, abs, waist..." (堆砌过多)
```

---

### 2.2.4 皮肤质感系统

#### A. 环境/状态增强（可选）

**寒冷环境：**
- `[Skin-Cold]` rosy cheeks from the cold（冻红的脸颊）

**战斗/户外：**
- `[Skin-Damage]` light scratches, smudges of dirt（轻微划痕、污迹）

---

#### B. 湿润质感模块（需逻辑场景）

**⚠️ 触发前提（必须符合以下场景之一）：**
- In the rain（雨中）
- Poolside / seaside（泳池边/海边）
- In the shower（淋浴中）
- After workout（运动后）
- Hot weather（炎热天气）

**基础状态：**
- wet skin, damp skin

**水分形态（可组合）：**

| 类型 | 关键词 |
|------|--------|
| 水珠 | water drops on skin, beads of water, water droplets |
| 汗珠 | beads of sweat, perspiration（仅运动/炎热场景） |
| 水流 | water running down her body, streaks of water |
| 薄膜 | thin film of water, glistening with moisture |

**光影互动（关键）：**
```
shiny skin, glistening skin, specular highlights on skin, 
dewy skin, oiled skin look, luminous skin
```

**完整示例：**
```
She stands under a sudden summer downpour, her skin glistening 
with water drops. Beads of water cling to her collarbones and 
run down her arms. Shiny skin with specular highlights catching 
the diffused light through rain clouds.
```

---

## 2.3 发型系统（Hairstyle System）

### 结构说明
- **默认基调**：及腰长发（waist-length long hair）+ 直发（straight, Type 1a/1b）
- **创意空间**：发质、造型、发色的多样化组合
- **避免单调**：高度鼓励使用造型变体

---

### 2.3.1 发质类型（增加真实感）

**用途**：打破"直发默认"，服务生活叙事

| 标签 | 发质类型 | 关键词 |
|------|----------|--------|
| `[Hair-Tex-1C]` | 粗直发 | coarse straight hair, high sheen |
| `[Hair-Tex-2B]` | S型波浪 | wavy, S-shaped curves, medium texture |
| `[Hair-Tex-3C]` | 螺旋卷 | tight corkscrew curls, high volume |
| `[Hair-Tex-4C]` | Z型紧密卷 | tightly coiled, Z-patterned, very dense |

---

### 2.3.2 发型长度与基础款式

**默认长度：**
- `[Hair-Len-Long]` waist-length long hair（及腰长发）

**日常功能性发型（可选）：**

| 标签 | 发型 | 关键词 |
|------|------|--------|
| `[Hair-Style-Bob]` | 蓬松鲍勃头 | shaggy bob, layered textured bob-length cut |
| `[Hair-Style-Lob]` | 锁骨直发 | lob / long bob, straight or wavy cut ending at collarbone |
| `[Hair-Style-Clip]` | 鲨鱼夹盘发 | claw clip updo, loosely twisted, pieces framing face |

---

### 2.3.3 造型变体（强烈推荐使用）

**⚠️ 规则**：在保留"长发"前提下，鼓励使用以下造型替代"自然披散"

#### A. 刘海造型

| 标签 | 类型 | 关键词 |
|------|------|--------|
| `[Hair-Bangs-Full]` | 齐刘海 | full bangs, blunt bangs |
| `[Hair-Bangs-Air]` | 空气刘海 | see-through air bangs, wispy bangs |
| `[Hair-Bangs-Curtain]` | 八字刘海 | curtain bangs, parted bangs |

---

#### B. 公主切

| 标签 | 类型 | 关键词 |
|------|------|--------|
| `[Hair-Hime]` | 公主切 | classic hime cut with long sidelocks |

---

#### C. 马尾造型

| 标签 | 类型 | 关键词 |
|------|------|--------|
| `[Hair-Pony-High]` | 高马尾 | high ponytail |
| `[Hair-Pony-Low]` | 低马尾 | low ponytail |
| `[Hair-Pony-Twin]` | 双马尾 | twin-tails |
| `[Hair-Pony-Side]` | 侧马尾 | side ponytail |

---

#### D. 编发造型

| 标签 | 类型 | 关键词 |
|------|------|--------|
| `[Hair-Braid-Single]` | 单麻花辫 | single braid |
| `[Hair-Braid-Fish]` | 鱼骨辫 | fishtail braid |
| `[Hair-Braid-Crown]` | 王冠式编发 | braided crown |
| `[Hair-Braid-Side]` | 侧边编发 | side braids |

---

#### E. 发髻造型

| 标签 | 类型 | 关键词 |
|------|------|--------|
| `[Hair-Bun-Odango]` | 双丸子头 | odango, twin buns |
| `[Hair-Bun-Single]` | 单丸子头 | single bun, top knot |

---

### 2.3.4 发型状态（瞬时叙事）

**用途**：捕捉生活瞬间，增强叙事性

| 标签 | 状态 | 关键词 | 适配场景 |
|------|------|--------|----------|
| `[Hair-State-Wet]` | 刚洗过 | freshly washed, damp, still slightly wet, clean texture | 浴室、清晨 |
| `[Hair-State-Wind]` | 被风吹乱 | windblown, messy, tousled, strands flying, full of motion | 户外、动态 |
| `[Hair-State-Sweat]` | 汗湿 | sweaty, matted, damp at roots and neck, clinging to skin | 运动后 |

---

### 2.3.5 发色设计系统（三步法）

**核心流程**：基础底色 + 挑染技术 + 亮点色系

---

#### 步骤1：选择基础底色

**自然色系：**

| 标签 | 颜色 | 关键词 |
|------|------|--------|
| `[Hair-Base-Black]` | 墨黑 | jet black, ink black |
| `[Hair-Base-Brown]` | 深棕/巧克力 | dark brown, chocolate |
| `[Hair-Base-Ash]` | 灰棕/蜜金 | ash brown, honey blonde |
| `[Hair-Base-Burgundy]` | 酒红/栗棕 | burgundy, auburn |

**幻想/浅色系：**

| 标签 | 颜色 | 关键词 |
|------|------|--------|
| `[Hair-Base-Platinum]` | 铂金 | platinum blonde |
| `[Hair-Base-Silver]` | 银白/灰 | silver white, ash grey |
| `[Hair-Base-Pink]` | 樱花粉 | sakura pink, pastel pink |
| `[Hair-Base-Blue]` | 天蓝 | sky blue, powder blue |
| `[Hair-Base-Lavender]` | 薰衣草紫 | lavender, lilac |

---

#### 步骤2：选择挑染技术（可选）

| 标签 | 技术 | 关键词 |
|------|------|--------|
| `[Hair-Dye-Highlight]` | 经典挑染 | classic highlights |
| `[Hair-Dye-Streak]` | 发片/区块染 | streaks, block dye, chunky highlights |
| `[Hair-Dye-Ombre]` | 渐变/退晕染 | ombré, balayage, gradient color |
| `[Hair-Dye-Under]` | 裙摆染/隐藏染 | under-dye, hidden layer dye, peek-a-boo highlights |

---

#### 步骤3：选择亮点色系（可选）

**高对比度色系：**
- platinum blonde, silver grey, fiery red, sapphire blue

**糖果幻想色系（重点推荐）：**
- cotton candy pink, mint green, baby blue, pastel lilac, lemon yellow, coral peach

**彩虹效果（多色组合）：**
```
示例：银白底色 + 裙摆染 + (粉+蓝+紫)糖果色
"silver-white hair with hidden layer dye in cotton candy pink, 
baby blue, and pastel lilac on the lower sections"
```

---

### 2.3.6 发型组合建议（避免单调）

**高频组合（需主动避开）：**
- ❌ 黑色长直发 + 自然披散（过于常见）
- ❌ 双马尾 + 粉色发（二次元刻板印象）

**创新组合示例：**
- ✅ 灰棕色 + 鱼骨辫 + 空气刘海
- ✅ 银白色 + 低马尾 + 裙摆染(薰衣草紫)
- ✅ 酒红色 + 公主切 + 卷发质感
- ✅ 天蓝色 + 鲨鱼夹盘发 + 垂落碎发

---

## 2.4 妆容系统（Makeup System）

### 核心哲学
- **叙事驱动**：妆容必须服务于角色设定和VIBE引擎
- **眼部优先**：重点刻画眼妆，放大吸引力
- **镜头关联**：面部特写时使用 close-up / medium close-up 确保细节

---

### 2.4.1 双轨美学分类

**主干道A：高级时尚奇观**
- 前卫、艺术性、视觉冲击力
- 适配：时尚摄影、奇观场景

**主干道B：生活叙事温度**
- 自然、日常、真实感
- 适配：市井场景、日常叙事

---

### 2.4.2 主干道A - 高级时尚妆容库

#### A1. 高级皮肤质感

| 标签 | 效果 | 关键词 |
|------|------|--------|
| `[Makeup-Skin-Glass]` | 玻璃肌 | flawless, poreless, luminous, intensely hydrated look |
| `[Makeup-Skin-Wet]` | 湿润肌 | high-shine, dewy, as if misted with water |
| `[Makeup-Skin-Gloss]` | 高光泽/油性 | reflective, editorial, slick finish on face and body |

---

#### A2. 面部装饰物

| 标签 | 类型 | 关键词 | 位置 |
|------|------|--------|------|
| `[Makeup-Deco-Crystal]` | 水晶/水钻 | crystals, rhinestones | near eyes, cheekbones, as freckles |
| `[Makeup-Deco-Pearl]` | 珍珠 | pearls adhered to face | tear-drops, along brows |
| `[Makeup-Deco-Foil]` | 金属箔片 | metallic foils, gold or silver | lips, eyes, brows |
| `[Makeup-Deco-Glitter]` | 亮片 | large chunky glitter, sequins | anywhere for texture |

---

#### A3. 前卫眼妆

| 标签 | 风格 | 关键词 |
|------|------|--------|
| `[Makeup-Eye-Graphic]` | 几何图形眼线 | graphic eyeliner, bold abstract shapes, non-traditional liner |
| `[Makeup-Eye-Float]` | 悬浮眼线 | floating crease liner, liner drawn above natural crease |
| `[Makeup-Eye-Block]` | 抽象色块 | abstract color blocking, bright eyeshadow as block of color |
| `[Makeup-Eye-Paint]` | 面部彩绘 | small artistic painted elements around eye |

---

#### A4. 前卫唇妆

| 标签 | 风格 | 关键词 |
|------|------|--------|
| `[Makeup-Lip-Vinyl]` | 黑胶光泽唇 | vinyl-inspired gloss, extremely high-shine, patent-leather look |
| `[Makeup-Lip-Metal]` | 金属质感唇 | metallic lips, chrome/gold/silver finish |
| `[Makeup-Lip-Bitten]` | 咬唇效果 | bitten lip stain, diffused just-bitten look, reds or berries |

---

#### A5. 亚文化风格（谨慎使用）

| 标签 | 风格 | 关键词 | 注意 |
|------|------|--------|------|
| `[Makeup-Goth]` | 哥特妆 | dark lipstick, heavy dark eyeliner, pale complexion | 避免过度使用 |
| `[Makeup-Punk]` | 朋克妆 | smudged heavy black eyes, bold unconventional shapes | 避免过度使用 |
| `[Makeup-Egirl]` | E-girl妆 | sharp winged liner, heavy blush on nose/cheeks, small hearts/dots under eyes | 注意年龄适配 |

---

### 2.4.3 主干道B - 生活自然妆容库

#### B1. "素净面容"妆容

| 标签 | 风格 | 关键词 |
|------|------|--------|
| `[Makeup-Natural-None]` | 无妆感妆容 | no-makeup makeup, enhances features, looks like bare skin |
| `[Makeup-Natural-Tint]` | 轻薄底妆 | sheer foundation, skin tint, freckles visible |
| `[Makeup-Natural-Brow]` | 自然眉 | lightly groomed brows, brushed up, slightly filled, not sculpted |
| `[Makeup-Natural-Blush]` | 自然腮红 | cream blush, natural flushed-from-within look |
| `[Makeup-Natural-Lip]` | 有色润唇 | tinted lip oil/balm, sheer color, healthy shine |

---

### 2.4.4 通用眼妆组件库（模块化组合）

**使用方式**：从4个层级中选择组件组合

---

#### 层级1：眼线风格

| 标签 | 风格 | 关键词 |
|------|------|--------|
| `[Eye-Liner-Cat]` | 经典猫眼 | classic cat-eye, winged eyeliner |
| `[Eye-Liner-Cleopatra]` | 埃及式 | Cleopatra style, thick black liner surrounding upper and lower lids, dramatic wing |
| `[Eye-Liner-Puppy]` | 无辜下垂眼线 | puppy-dog style, downturned eyeliner for innocent look |

---

#### 层级2：睫毛形态

| 标签 | 形态 | 关键词 |
|------|------|--------|
| `[Eye-Lash-Volume]` | 浓密卷翘 | voluminous upper lashes, thick curled false eyelashes |
| `[Eye-Lash-Long]` | 纤长 | long wispy eyelashes, extended upper lashes |
| `[Eye-Lash-Anime]` | 动漫下睫毛 | anime-style lower lashes, clustered defined bottom lashes |

---

#### 层级3：瞳孔与卧蚕

| 标签 | 类型 | 关键词 |
|------|------|--------|
| `[Eye-Lens-Color]` | 彩色美瞳 | colored contact lenses, vivid circle lenses, ice-blue eyes, emerald green eyes |
| `[Eye-Aegyo]` | 卧蚕提亮 | highlighted aegyo-sal, shimmering under-eye, highlighted tear duct |

---

#### 层级4：眼影风格

| 标签 | 风格 | 关键词 |
|------|------|--------|
| `[Eye-Shadow-Smoky]` | 经典烟熏 | classic smoky eyes, blended dark eyeshadow |
| `[Eye-Shadow-Metal]` | 金属/珠光 | metallic eyeshadow, glittering eyelids, duochrome eyeshadow, shimmer texture |

---

### 2.4.5 妆容组合建议

**高频组合（需避开）：**
- ❌ 猫眼线 + 红唇（过于经典/常见）
- ❌ 烟熏妆 + 黑唇（哥特刻板印象）

**创新组合示例：**
- ✅ 悬浮眼线 + 玻璃唇 + 珍珠装饰（时尚前卫）
- ✅ 自然眉 + 奶油腮红 + 有色润唇（日常清新）
- ✅ 几何眼线 + 金属唇 + 水晶装饰（未来主义）
- ✅ 无妆感底妆 + 卧蚜提亮 + 淡粉唇（纯欲少女）

---

## 2.5 纹身系统（Tattoo System）

### ⚠️ 重要说明
纹身是高级叙事工具，但使用频率应控制。建议每20个创意中使用不超过3次。

---

### 2.5.1 核心哲学

**本体论定义：**
- 纹身是"角色的第二层皮肤"和"人格锚点"
- 严禁作为廉价装饰或随机视觉噪音
- 必须服务于"核心创伤"、"信仰体系"或"社会面具"

**叙事功能：**
- **展示（Reveal）**：公开宣言，昭示身份
- **防御（Protect）**：私密护身符，抵御创伤

---

### 2.5.2 位置规范与解剖学流向

#### A. S形曲线法则
- 大面积纹身必须顺应肌肉骨骼的自然起伏
- 严禁僵硬地将矩形图像"贴"在圆柱状肢体上
- 动态姿势时，纹身随肌肉拉伸产生有机形变

---

#### B. 痛觉仪式与区域分级

**Level A：公共宣言区**

| 标签 | 位置 | 关键词 | 叙事功能 |
|------|------|--------|----------|
| `[Tattoo-Forearm]` | 前臂 | forearm tattoo | 社会身份展示，箴言、图腾 |
| `[Tattoo-Neck]` | 颈侧 | neck side tattoo | 无畏宣言，职业标识 |

**Level B：私密图腾区**

| 标签 | 位置 | 关键词 | 叙事功能 |
|------|------|--------|----------|
| `[Tattoo-Sternum]` | 胸骨/下乳 | sternum/underboob tattoo | 核心价值观，曼陀罗、护身符 |
| `[Tattoo-Ribs]` | 肋骨 | rib tattoo | 私密日记，纪念逝者文字 |

**Level C：大面积叙事区**

| 标签 | 位置 | 关键词 | 叙事功能 |
|------|------|--------|----------|
| `[Tattoo-Spine]` | 脊柱 | spine tattoo | 能量中轴，垂直书法、线性图腾 |
| `[Tattoo-Back]` | 整个背部 | full back tattoo | 史诗叙事，东方龙、西方神话 |
| `[Tattoo-Sleeve]` | 整臂 | full sleeve tattoo | 时间线叙事，花卉、机械、几何 |
| `[Tattoo-Leg]` | 大腿 | thigh tattoo | 隐藏的权力，蛇、藤蔓、宗教 |

---

### 2.5.3 风格分类

| 标签 | 风格 | 关键词 | 视觉特征 |
|------|------|--------|----------|
| `[Tattoo-East]` | 东方传统 | oriental traditional tattoo, dragon, koi, phoenix, lotus | 大面积、浓墨重彩 |
| `[Tattoo-Tribal]` | 部落图腾 | tribal tattoo, geometric patterns, black bold lines | 抽象、对称、黑色 |
| `[Tattoo-Realism]` | 写实主义 | realistic tattoo, portrait, animal, landscape | 照片级细节 |
| `[Tattoo-Geometry]` | 几何 | geometric tattoo, sacred geometry, mandala | 精确线条、对称 |
| `[Tattoo-Watercolor]` | 水彩 | watercolor tattoo, splashes of color, soft edges | 彩色、柔和边缘 |
| `[Tattoo-Script]` | 书法/文字 | script tattoo, calligraphy, quote, date | 优雅字体、个人意义 |
| `[Tattoo-Floral]` | 花卉 | floral tattoo, rose, peony, cherry blossom | 女性化、柔美 |
| `[Tattoo-Blackwork]` | 黑作 | blackwork tattoo, solid black fill, negative space | 高对比、现代感 |

---

### 2.5.4 使用建议

**何时使用纹身：**
- ✅ 角色有明确的"身份标签"（摇滚乐手、帮派成员、叛逆者）
- ✅ 需要视觉锚点强化"反差"（如：纹身少女 + 婚纱）
- ✅ 服务于"引擎C：概念内核"的哲学叙事

**何时不使用纹身：**
- ❌ 清纯、学生、职场OL等常规身份
- ❌ 已经有足够视觉元素（复杂服装 + 复杂场景）
- ❌ 只是为了"增加细节"而添加

---

## 📊 角色系统组合速查表

### 快速组合公式

```
完整角色 = 面部基底 + [体型微调] + 发型 + 妆容 + [可选纹身]
```

### 典型组合示例

**组合1：清纯学生**
```
- 面部：东亚基底 + 大眼睛 + 小翘鼻
- 体型：纤细骨感
- 发型：黑色长直发 + 空气刘海
- 妆容：无妆感 + 自然眉 + 有色润唇
- 纹身：无
```

**组合2：时尚前卫**
```
- 面部：东亚基底 + 琥珀瞳 + 微驼峰鼻
- 体型：沙漏曲线 + 突出锁骨
- 发型：银白色 + 裙摆染(粉紫) + 低马尾
- 妆容：玻璃肌 + 几何眼线 + 金属唇 + 水晶装饰
- 纹身：无或颈侧小型图腾
```

**组合3：运动活力**
```
- 面部：东亚基底 + 丹凤眼
- 体型：运动健美 + 马甲线
- 发型：高马尾 + 荧光发带
- 妆容：自然底妆 + 卧蚕提亮 + 淡色润唇
- 纹身：无
```

**组合4：叛逆摇滚**
```
- 面部：东亚基底 + 浅色瞳孔
- 体型：沙漏曲线 + 美背
- 发型：酒红色 + 区块染(银) + 蓬松波浪
- 妆容：烟熏妆 + 朋克风 + 黑唇
- 纹身：整臂花卉纹身
```

---

## 🎯 使用提示

### 1. 避免堆砌
```
❌ 错误："featuring swan neck, collarbones, abs, long legs, 
     with tattoos on forearm, ribs, and spine..."

✅ 正确："featuring prominent collarbones, wearing off-shoulder gown"
```

### 2. 保持一致性
```
❌ 不协调："清纯学生 + 烟熏妆 + 整臂纹身"

✅ 协调："清纯学生 + 无妆感 + 空气刘海"
```

### 3. 服务叙事
```
每个选择都应回答："这个元素如何强化角色故事？"

示例：
- 选择马甲线 → 配合运动场景
- 选择纹身 → 配合叛逆/亚文化身份
- 选择玻璃肌 → 配合高级时尚场景
```

---

## 结语

角色系统是整个创意的"锚点"。合理组合这些模块，可以创造出：
- **辨识度高**：通过微调避免千人一面
- **叙事性强**：每个元素服务于角色设定
- **美学平衡**：不过度堆砌，保持克制

下一步：服装系统、场景系统、VIBE引擎的重组优化。
