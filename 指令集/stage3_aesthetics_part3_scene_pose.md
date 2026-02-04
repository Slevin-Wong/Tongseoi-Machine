# 阶段三：美学库重组（v2.0）- 第三部分：场景与姿态系统

---

## 📋 说明

本文档覆盖：
- **第四部分 - 场景系统**（环境、构图、光影、氛围）
- **第五部分 - 姿态系统**（单人姿态、互动叙事）

---

## 🌍 第四部分：场景系统（Scene System）

### 快速导航
- [4.1 场景环境库](#41-场景环境库) - 室内、室外、特殊场景
- [4.2 构图与镜头](#42-构图与镜头) - 景别、角度、构图法则
- [4.3 光影系统](#43-光影系统) - 光源、色调、特殊光效
- [4.4 氛围填充](#44-氛围填充) - 介质、粒子、细节

---

## 4.1 场景环境库（Environment Library）

### 4.1.0 场景选择协议（反套路）

**核心原则**：避免"显而易见"的组合

**高频套路（需避开）：**
- ❌ 汉服 + 古建筑园林
- ❌ 运动装 + 健身房
- ❌ 婚纱 + 教堂/海滩
- ❌ 哥特服饰 + 废墟/墓地

**创新策略**：
- ✅ 文化服饰 + 现代场景（如：汉服 + 地铁站）
- ✅ 华丽服饰 + 简陋场景（如：礼服 + 便利店）
- ✅ 休闲服装 + 宏大场景（如：T恤 + 宫殿）

---

### 4.1.1 自然环境

#### A. 森林与植被

| 标签 | 场景 | 关键词 | 氛围 |
|------|------|--------|------|
| `[Scene-Forest-Deep]` | 深林 | deep forest, dense trees, dappled sunlight, moss-covered | 神秘、静谧 |
| `[Scene-Forest-Birch]` | 白桦林 | birch forest, white tree trunks, delicate leaves | 清新、梦幻 |
| `[Scene-Forest-Bamboo]` | 竹林 | bamboo forest, tall bamboo stalks, filtered green light | 东方、禅意 |
| `[Scene-Jungle]` | 丛林 | jungle, tropical plants, vines, humid atmosphere | 原始、野性 |
| `[Scene-Meadow]` | 草地/花海 | wildflower meadow, rolling hills, open sky | 明快、浪漫 |

---

#### B. 水域环境

| 标签 | 场景 | 关键词 | 氛围 |
|------|------|--------|------|
| `[Scene-Beach]` | 海滩 | sandy beach, ocean waves, horizon, seashells | 清爽、度假 |
| `[Scene-Seaside-Cliff]` | 海边悬崖 | coastal cliff, crashing waves, rocky outcrop | 壮阔、孤独 |
| `[Scene-Lake]` | 湖泊 | calm lake, reflective water, surrounding nature | 平静、诗意 |
| `[Scene-River]` | 河流/溪流 | flowing river, smooth stones, ripples | 灵动、清新 |
| `[Scene-Waterfall]` | 瀑布 | waterfall, mist, cascading water, rocks | 磅礴、动态 |
| `[Scene-Pond]` | 池塘 | small pond, lotus flowers, lily pads | 静谧、东方 |

---

#### C. 山地与天空

| 标签 | 场景 | 关键词 | 氛围 |
|------|------|--------|------|
| `[Scene-Mountain]` | 山脉 | mountain range, peaks, valley, dramatic landscape | 宏伟、壮丽 |
| `[Scene-Hilltop]` | 山顶/丘陵 | hilltop, panoramic view, wind, clouds | 开阔、自由 |
| `[Scene-Canyon]` | 峡谷 | canyon, layered rock, deep gorge | 雄浑、原始 |
| `[Scene-Desert]` | 沙漠 | desert, sand dunes, endless horizon, heat shimmer | 孤寂、极简 |
| `[Scene-Sky]` | 天空场景 | open sky, clouds, sunset/sunrise, vast | 空灵、自由 |

---

#### D. 季节性场景

| 标签 | 场景 | 关键词 | 氛围 |
|------|------|--------|------|
| `[Scene-Spring]` | 春季场景 | cherry blossoms, fresh green, gentle breeze | 生机、浪漫 |
| `[Scene-Summer]` | 夏季场景 | bright sunlight, lush greenery, vibrant colors | 热烈、明快 |
| `[Scene-Autumn]` | 秋季场景 | fallen leaves, golden foliage, crisp air | 怀旧、温暖 |
| `[Scene-Winter]` | 冬季场景 | snow-covered, frost, bare trees, cold | 纯净、寂静 |

---

### 4.1.2 城市环境

#### A. 现代都市

| 标签 | 场景 | 关键词 | 氛围 |
|------|------|--------|------|
| `[Scene-City-Street]` | 都市街道 | urban street, skyscrapers, neon signs, pedestrians | 繁华、现代 |
| `[Scene-City-Alley]` | 小巷 | narrow alley, brick walls, puddles, intimate | 私密、城市肌理 |
| `[Scene-City-Rooftop]` | 天台/屋顶 | rooftop, city skyline view, edge, wind | 孤独、俯瞰 |
| `[Scene-City-Subway]` | 地铁站 | subway platform, fluorescent lights, tiles, crowd | 都市、日常 |
| `[Scene-City-Bridge]` | 桥梁 | bridge, river below, city lights, architecture | 连接、过渡 |

---

#### B. 商业/公共空间

| 标签 | 场景 | 关键词 | 氛围 |
|------|------|--------|------|
| `[Scene-Shop-Cafe]` | 咖啡馆 | cozy cafe, wooden tables, coffee aroma, warm lights | 温馨、文艺 |
| `[Scene-Shop-Book]` | 书店 | bookstore, shelves of books, quiet atmosphere | 知性、静谧 |
| `[Scene-Shop-Vintage]` | 古董/唱片店 | vintage shop, retro items, nostalgic vibe | 怀旧、复古 |
| `[Scene-Shop-Convenience]` | 便利店 | convenience store, fluorescent lights, shelves, urban | 日常、都市 |
| `[Scene-Mall]` | 购物中心 | shopping mall, bright lights, modern architecture | 消费、现代 |

---

#### C. 交通枢纽

| 标签 | 场景 | 关键词 | 氛围 |
|------|------|--------|------|
| `[Scene-Train-Station]` | 火车站 | train station, platform, departure boards, travelers | 离别、旅程 |
| `[Scene-Airport]` | 机场 | airport terminal, glass walls, luggage, journey | 现代、过渡 |
| `[Scene-Bus-Stop]` | 公交站 | bus stop, shelter, waiting, urban | 日常、等待 |

---

#### D. 娱乐场所

| 标签 | 场景 | 关键词 | 氛围 |
|------|------|--------|------|
| `[Scene-Club]` | 夜店/酒吧 | nightclub, dim lights, dance floor, music | 热烈、夜生活 |
| `[Scene-Theater]` | 剧院 | theater, stage, red curtains, seats | 艺术、表演 |
| `[Scene-Cinema]` | 电影院 | cinema, screen, seats, dark | 怀旧、静谧 |
| `[Scene-Arcade]` | 游戏厅 | arcade, neon games, retro atmosphere | 怀旧、青春 |

---

### 4.1.3 室内环境

#### A. 居住空间

| 标签 | 场景 | 关键词 | 氛围 |
|------|------|--------|------|
| `[Scene-Room-Bedroom]` | 卧室 | bedroom, bed, soft lighting, personal space | 私密、温暖 |
| `[Scene-Room-Living]` | 客厅 | living room, sofa, windows, natural light | 日常、舒适 |
| `[Scene-Room-Kitchen]` | 厨房 | kitchen, cooking, morning light, homey | 生活、温馨 |
| `[Scene-Room-Bathroom]` | 浴室 | bathroom, bathtub, steam, tiles, mirror | 私密、放松 |
| `[Scene-Room-Balcony]` | 阳台 | balcony, plants, city view, breeze | 过渡、休憩 |

---

#### B. 工作/学习空间

| 标签 | 场景 | 关键词 | 氛围 |
|------|------|--------|------|
| `[Scene-Office]` | 办公室 | office, desk, computer, professional | 职业、现代 |
| `[Scene-Library]` | 图书馆 | library, bookshelves, reading tables, quiet | 知识、静谧 |
| `[Scene-Classroom]` | 教室 | classroom, desks, blackboard, windows | 青春、学习 |
| `[Scene-Studio]` | 工作室/画室 | art studio, easel, creative mess, natural light | 艺术、创造 |

---

#### C. 特殊室内

| 标签 | 场景 | 关键词 | 氛围 |
|------|------|--------|------|
| `[Scene-Church]` | 教堂 | church interior, stained glass, pews, sacred | 神圣、庄严 |
| `[Scene-Museum]` | 博物馆 | museum, exhibits, marble floors, art | 文化、静谧 |
| `[Scene-Ballroom]` | 舞厅/宫殿 | grand ballroom, chandeliers, marble, luxurious | 奢华、盛大 |
| `[Scene-Greenhouse]` | 温室 | greenhouse, glass panels, plants, humid | 生机、梦幻 |

---

### 4.1.4 特殊/废弃环境

#### A. 工业废墟

| 标签 | 场景 | 关键词 | 氛围 |
|------|------|--------|------|
| `[Scene-Factory]` | 废弃工厂 | abandoned factory, rusted machinery, broken windows | 荒凉、时间 |
| `[Scene-Warehouse]` | 仓库 | empty warehouse, concrete, metal beams, echoing | 空旷、冷硬 |
| `[Scene-Station-Old]` | 废弃车站 | old train station, overgrown tracks, nostalgia | 怀旧、遗弃 |

**⚠️ 使用建议**：
- 废墟场景是"显性元素"，避免与哥特服饰固定搭配
- 推荐与华丽服饰组合，创造反差（解耦原则）

---

#### B. 建筑遗迹

| 标签 | 场景 | 关键词 | 氛围 |
|------|------|--------|------|
| `[Scene-Ruins-Ancient]` | 古代遗迹 | ancient ruins, stone columns, weathered | 历史、沧桑 |
| `[Scene-Castle]` | 城堡 | castle, stone walls, towers, medieval | 古典、神秘 |
| `[Scene-Manor]` | 庄园/大宅 | old manor, overgrown garden, vintage | 贵族、衰败 |

---

### 4.1.5 幻想/建构场景（引擎E专用）

**⚠️ 使用前提**：必须遵守"可推演"原则，有现实锚点

| 标签 | 场景 | 现实锚点 | 关键词 |
|------|------|----------|--------|
| `[Scene-Eco-City]` | 生态城市 | 气候应对、垂直农场 | green architecture, vertical gardens, sustainable |
| `[Scene-Float-Garden]` | 悬浮花园 | 工程可能性、大型装置 | floating platforms, suspended greenery, cables |
| `[Scene-Water-City]` | 水城 | 海平面上升应对 | elevated walkways, buildings on stilts, canals |
| `[Scene-Ice-Structure]` | 冰建筑 | 季节性结晶、气候利用 | ice architecture, frozen structures, temporary |

---

## 4.2 构图与镜头（Composition & Camera）

### 4.2.1 景别系统（Shot Size）

**✅ 允许使用：**

| 标签 | 景别 | 关键词 | 用途 |
|------|------|--------|------|
| `[Shot-CU]` | 特写 | close-up, face-focused, intimate | 表情、妆容细节 |
| `[Shot-MCU]` | 中特写 | medium close-up, head and shoulders | 面部 + 上身 |
| `[Shot-MS]` | 中景 | medium shot, waist up | 姿态 + 服装上半 |
| `[Shot-FS]` | 全景 | full shot, entire body visible | 全身造型 + 姿态 |

**🔴 严禁使用：**
- ❌ long shot（远景）
- ❌ extreme long shot（极远景）
- ❌ wide shot（如果指全景远景）

**原因**：远景会导致面部细节崩坏

---

### 4.2.2 拍摄角度（Camera Angle）

| 标签 | 角度 | 关键词 | 效果 |
|------|------|--------|------|
| `[Angle-Eye]` | 平视 | eye-level angle, neutral perspective | 自然、客观 |
| `[Angle-Low]` | 低角度/仰视 | low angle, looking up, empowering | 权威、高大 |
| `[Angle-High]` | 高角度/俯视 | high angle, looking down, delicate | 柔弱、可爱 |
| `[Angle-Dutch]` | 荷兰角/倾斜 | dutch angle, tilted, dynamic | 不安、动态 |
| `[Angle-Over-Shoulder]` | 过肩视角 | over-the-shoulder view, side profile visible | 叙事、互动 |

---

### 4.2.3 构图法则

#### A. 经典构图

| 标签 | 法则 | 关键词 | 说明 |
|------|------|--------|------|
| `[Comp-Rule-Thirds]` | 三分法则 | rule of thirds, off-center subject | 动态平衡 |
| `[Comp-Center]` | 中心构图 | centered composition, symmetrical | 稳定、庄重 |
| `[Comp-Frame]` | 框架构图 | natural framing, doorway, window | 聚焦、层次 |
| `[Comp-Leading]` | 引导线 | leading lines, perspective, depth | 引导视线 |
| `[Comp-Diagonal]` | 对角线 | diagonal composition, dynamic | 动感、张力 |

---

#### B. 强制分层（重要）

**核心要求**：所有图像必须包含清晰的前景、中景、背景

**分层元素示例：**

```
前景（Foreground）：
- 失焦的花瓣、叶子
- 模糊的栏杆、窗框
- 景深虚化的物体

中景（Midground）：
- 主体人物
- 主要互动对象
- 核心叙事元素

背景（Background）：
- 环境场景
- 建筑、天空
- 氛围渲染
```

**示例描述：**
```
In the foreground, out-of-focus purple lupines. In the midground, 
the model stands centered. In the background, a distant birch forest 
fades into soft focus.
```

---

## 4.3 光影系统（Lighting System）

### 4.3.1 自然光源

#### A. 时间导向

| 标签 | 光线 | 关键词 | 色调 |
|------|------|--------|------|
| `[Light-Dawn]` | 黎明 | dawn light, pre-sunrise, soft blue-purple | 冷静、希望 |
| `[Light-Morning]` | 晨光 | morning light, fresh, clear, gentle | 清新、温暖 |
| `[Light-Noon]` | 正午 | harsh midday sun, strong shadows, bright | 强烈、明快 |
| `[Light-Golden]` | 黄金时刻 | golden hour, warm glow, soft shadows | 浪漫、温暖 |
| `[Light-Dusk]` | 黄昏 | dusk, fading light, orange-pink sky | 怀旧、柔和 |
| `[Light-Night]` | 夜晚 | moonlight, starlight, dim, cool | 神秘、冷清 |

---

#### B. 天气导向

| 标签 | 光线 | 关键词 | 氛围 |
|------|------|--------|------|
| `[Light-Overcast]` | 阴天 | overcast, diffused light, soft shadows | 柔和、忧郁 |
| `[Light-Rainy]` | 雨天 | rainy, wet surfaces, reflections | 清新、情绪 |
| `[Light-Foggy]` | 雾气 | foggy, mist, reduced visibility, ethereal | 梦幻、神秘 |
| `[Light-Sunny]` | 晴天 | bright sunshine, clear sky, vibrant | 明快、活力 |

---

### 4.3.2 人工光源

#### A. 室内照明

| 标签 | 光源 | 关键词 | 氛围 |
|------|------|--------|------|
| `[Light-Window]` | 窗光 | window light, soft diffused, natural | 柔和、日常 |
| `[Light-Lamp]` | 台灯/落地灯 | warm lamp light, cozy, intimate | 温馨、私密 |
| `[Light-Candle]` | 烛光 | candlelight, flickering, romantic | 浪漫、柔和 |
| `[Light-Fluorescent]` | 荧光灯 | fluorescent light, cold, institutional | 冷硬、都市 |

---

#### B. 城市照明

| 标签 | 光源 | 关键词 | 氛围 |
|------|------|--------|------|
| `[Light-Neon]` | 霓虹灯 | neon signs, colorful glow, urban | 都市、夜生活 |
| `[Light-Street]` | 路灯 | street lamps, warm pools of light, shadows | 夜晚、都市 |
| `[Light-LED]` | LED屏幕 | LED screens, digital glow, modern | 科技、现代 |

---

### 4.3.3 光影技法

#### A. 光线方向

| 标签 | 方向 | 关键词 | 效果 |
|------|------|--------|------|
| `[Light-Dir-Front]` | 正面光 | frontal lighting, even illumination | 明亮、平面 |
| `[Light-Dir-Side]` | 侧光 | side lighting, dramatic shadows, contour | 立体、戏剧 |
| `[Light-Dir-Back]` | 逆光/背光 | backlighting, rim light, silhouette | 轮廓、梦幻 |
| `[Light-Dir-Top]` | 顶光 | top lighting, harsh shadows under features | 强烈、不常用 |

---

#### B. 光影特效

| 标签 | 特效 | 关键词 | 视觉效果 |
|------|------|--------|----------|
| `[Light-God-Ray]` | 丁达尔效应/上帝之光 | god rays, volumetric light, beams through dust/mist | 神圣、戏剧化 |
| `[Light-Dappled]` | 斑驳光影 | dappled light, light filtering through leaves | 自然、梦幻 |
| `[Light-Reflection]` | 反射光 | reflected light, bounce light, soft fill | 柔和、间接 |
| `[Light-Specular]` | 高光 | specular highlights, shiny surfaces, catchlights | 质感、细节 |

---

### 4.3.4 色调与氛围

#### A. 色温

| 标签 | 色调 | 关键词 | 情绪 |
|------|------|--------|------|
| `[Tone-Warm]` | 暖色调 | warm tones, golden, orange, cozy | 温暖、怀旧 |
| `[Tone-Cool]` | 冷色调 | cool tones, blue, cyan, crisp | 冷静、现代 |
| `[Tone-Neutral]` | 中性色调 | neutral white balance, balanced | 自然、真实 |

---

#### B. 饱和度与对比

| 标签 | 风格 | 关键词 | 效果 |
|------|------|--------|------|
| `[Tone-High-Contrast]` | 高对比 | high contrast, deep shadows, bright highlights | 强烈、戏剧 |
| `[Tone-Low-Contrast]` | 低对比 | low contrast, soft, muted | 柔和、梦幻 |
| `[Tone-Saturated]` | 高饱和 | saturated colors, vibrant, vivid | 明快、活力 |
| `[Tone-Desaturated]` | 低饱和 | desaturated, muted colors, soft | 复古、忧郁 |

---

## 4.4 氛围填充（Atmospheric Filling）

### 4.4.1 核心哲学

**原则**：空间永远不是"空"的

**目标**：通过"介质"填充负空间，创造体积感和沉浸感

**禁令**：
- ❌ 严禁"空虚"背景（纯色块、无尽虚空）
- ✅ 即使极简场景，也必须包含结构细节

---

### 4.4.2 填充工具箱

#### A. 悬浮微粒

| 标签 | 粒子 | 关键词 | 适用场景 |
|------|------|--------|----------|
| `[Atmos-Dust]` | 灰尘 | dust particles, suspended in air, visible in light beams | 室内、废墟 |
| `[Atmos-Petals]` | 花瓣 | flower petals, drifting, floating | 春季、浪漫 |
| `[Atmos-Leaves]` | 落叶 | falling leaves, autumn, swirling | 秋季、怀旧 |
| `[Atmos-Snow]` | 雪花 | snowflakes, gentle fall, winter | 冬季、纯净 |
| `[Atmos-Embers]` | 余烬 | embers, glowing, rising | 火、温暖 |
| `[Atmos-Bubbles]` | 气泡 | soap bubbles, floating, iridescent | 梦幻、童趣 |

---

#### B. 气态流体

| 标签 | 介质 | 关键词 | 视觉效果 |
|------|------|--------|----------|
| `[Atmos-Fog]` | 浓雾 | thick fog, obscured visibility, mystery | 神秘、梦幻 |
| `[Atmos-Mist]` | 晨霭/薄雾 | morning mist, light fog, ethereal | 柔和、清新 |
| `[Atmos-Smoke]` | 烟雾 | smoke, colored smoke, swirling | 戏剧化、动态 |
| `[Atmos-Steam]` | 蒸汽 | steam, rising, warm | 温暖、柔和 |
| `[Atmos-Haze]` | 雾霭/霾 | haze, atmospheric perspective, depth | 深度、距离 |

---

#### C. 有机覆盖

| 标签 | 元素 | 关键词 | 适用场景 |
|------|------|--------|----------|
| `[Atmos-Vines]` | 藤蔓 | climbing vines, overgrown, green | 废墟、自然 |
| `[Atmos-Moss]` | 苔藓 | moss-covered, green texture, damp | 森林、古迹 |
| `[Atmos-Flowers-Wild]` | 野花 | wildflowers, scattered, colorful | 草地、自然 |
| `[Atmos-Ivy]` | 常春藤 | ivy, covering walls, green | 建筑、古典 |

---

#### D. 物品堆叠

| 标签 | 物品 | 关键词 | 适用场景 |
|------|------|--------|----------|
| `[Atmos-Books]` | 书籍 | stacks of books, scattered pages | 图书馆、书房 |
| `[Atmos-Candles]` | 蜡烛 | multiple candles, flickering flames | 浪漫、神秘 |
| `[Atmos-Lanterns]` | 灯笼 | hanging lanterns, warm glow | 东方、节日 |
| `[Atmos-Papers]` | 纸张 | scattered papers, documents | 办公、混乱 |

**⚠️ 禁令提醒**：
- ❌ 避免"桌上摆满杂物"（table covered in many small objects）
- ✅ 使用有序的物品堆叠，保持视觉清晰度

---

### 4.4.3 动态环境元素

#### A. 天气效果

| 标签 | 天气 | 关键词 | 动态感 |
|------|------|--------|--------|
| `[Weather-Rain]` | 雨 | rain, falling droplets, wet surfaces | 清新、动态 |
| `[Weather-Wind]` | 风 | strong wind, hair and clothes blowing | 动感、力量 |
| `[Weather-Thunder]` | 雷电 | thunder and lightning, dramatic sky | 戏剧、紧张 |
| `[Weather-Snow]` | 降雪 | falling snow, accumulation, cold | 宁静、冬季 |

**⚠️ 禁令提醒**：
- ❌ 避免"龙卷风"（tornado）等极端天气（除非引擎E有合理锚点）

---

#### B. 光学现象

| 标签 | 现象 | 关键词 | 效果 |
|------|------|--------|------|
| `[Optical-Rainbow]` | 彩虹 | rainbow, arc of colors, after rain | 希望、美丽 |
| `[Optical-Sunset]` | 晚霞 | sunset glow, colorful sky, warm | 浪漫、壮丽 |
| `[Optical-Aurora]` | 极光 | aurora, northern lights, dancing colors | 神奇、罕见 |
| `[Optical-Lens-Flare]` | 镜头光晕 | lens flare, sun glare, bright spots | 真实感、光线 |

---

## 💡 场景系统组合示例

### 示例1：自然清新（主干道B）
```
场景：白桦林（[Scene-Forest-Birch]）
光影：晨光（[Light-Morning]）+ 斑驳光影（[Light-Dappled]）
氛围：薄雾（[Atmos-Mist]）+ 飘落花瓣（[Atmos-Petals]）
构图：三分法则（[Comp-Rule-Thirds]）+ 前景失焦野花
镜头：中景（[Shot-MS]）+ 平视（[Angle-Eye]）

描述：
"Medium shot at eye-level in a birch forest. Morning light filters 
through white tree trunks creating dappled shadows. Thin mist hangs 
in the air. In the foreground, out-of-focus wildflowers. Sakura petals 
drift gently. The model stands among birch trees, rule of thirds composition."
```

---

### 示例2：都市霓虹（主干道A）
```
场景：都市天台（[Scene-City-Rooftop]）
光影：夜晚（[Light-Night]）+ 霓虹灯（[Light-Neon]）+ 背光（[Light-Dir-Back]）
氛围：轻雾（[Atmos-Mist]）+ 雨后湿润（[Weather-Rain]）
构图：低角度（[Angle-Low]）+ 对角线（[Comp-Diagonal]）
镜头：全景（[Shot-FS]）

描述：
"Full shot from low angle on a city rooftop at night. Neon signs 
from surrounding buildings cast colorful backlighting. Light mist 
in the air. Wet surfaces reflect neon colors. City skyline in the 
background. Diagonal composition with the model standing at the edge."
```

---

### 示例3：废墟华丽（解耦/反差）
```
场景：废弃工厂（[Scene-Factory]）
光影：侧光（[Light-Dir-Side]）+ 上帝之光（[Light-God-Ray]）
氛围：粉尘（[Atmos-Dust]）+ 藤蔓（[Atmos-Vines]）
构图：框架构图（[Comp-Frame]）+ 中心对称
镜头：中特写（[Shot-MCU]）

描述：
"Medium close-up in an abandoned factory. Harsh side lighting from 
broken windows creates dramatic god rays cutting through dust particles. 
Vines creep through cracks. Rusted metal beams frame the composition. 
The model centered, wearing an elegant gown in stark contrast to the 
industrial decay."
```

---

## 🎯 场景系统使用提示

### 1. 避免"空虚"场景
```
❌ 错误：
"standing in a white room"

✅ 正确：
"standing in a minimalist white room with concrete texture walls, 
geometric shadows cast by hidden skylights, and subtle dust particles 
visible in light beams"
```

---

### 2. 强制分层
```
每个场景必须包含：
☐ 前景元素（失焦或框架）
☐ 中景主体（人物 + 核心叙事）
☐ 背景环境（场景深度）
```

---

### 3. 氛围介质
```
检查清单：
☐ 空气中是否有"填充物"？（雾、尘、花瓣等）
☐ 光线是否可视化？（通过介质产生体积光）
☐ 环境是否有"质感"？（不只是色块）
```

---

## 🤸 第五部分：姿态系统（Pose & Interaction System）

### 快速导航
- [5.1 单人姿态](#51-单人姿态) - 手部、腿部、视角
- [5.2 互动叙事](#52-互动叙事) - 人物互动、动物互动

---

## 5.1 单人姿态（Solo Posing）

### 5.1.1 核心原则

**解放动态与表现力：**
- 鼓励复杂、动态、富有表现力的姿势
- 跑、跳、舞蹈、战斗等动态瞬间允许
- 前提：增强画面概念和美学价值

**姿态与局部美学联动：**
- 姿态选择应服务于[2.2.2 局部美学]焦点
- 例如：选择"突出锁骨" → 使用露肩姿态

---

### 5.1.2 视角与体态原则

#### A. 视角与身体焦点联动

**正面/四分之三视角（Front / 3/4 View）：**
- 适合展示：锁骨、胸部轮廓、腹肌
- 关键词：`frontal view, three-quarter view, facing camera`

**侧面/背面视角（Side / Back View）：**
- 适合展示：美背线条、臀部曲线
- 关键词：`side view, back view, profile`

**通用焦点：**
- 长腿、细腰：多角度适用

---

#### B. 背视回眸法则（重要）

**🔴 强制规则**：背对镜头时，必须通过回眸与观众建立情感连接

**严禁**：只留后脑勺

**关键词：**
```
looking back over her shoulder at the camera
glancing back with a smile
a stunning backward glance
revealing her perfect side profile
```

---

### 5.1.3 手部姿态库（Hand Gesture Library）

#### 分类A：积极与正面情绪

**A1. 可爱（Cute）**

| 标签 | 姿态 | 关键词 |
|------|------|--------|
| `[Hand-Cat-Paw]` | 猫爪式 | imitating cat paws, hands near cheek/lips/chin |
| `[Hand-Flower-Cup]` | 花萼式 | hands clasped under chin, cupping face like flower bud |
| `[Hand-Fist-Cheek]` | 小拳头抵脸 | gently clenched fist, knuckles resting on cheek/lips |
| `[Hand-Poke-Cheek]` | 单指点脸颊 | index finger gently poking own cheek, head tilt |
| `[Hand-Eye-Frame]` | 框住眼睛 | making circle/OK sign, placing over one eye |

---

**A2. 俏皮（Playful）**

| 标签 | 姿态 | 关键词 |
|------|------|--------|
| `[Hand-Salute]` | 随意敬礼 | casual salute, relaxed, informal |
| `[Hand-Pull-Hair]` | 拉扯发辫/衣角 | lightly pinching hair tip, collar, hat brim |
| `[Hand-Shh]` | "嘘"声手势 | index finger vertical in front of lips, sharing secret |
| `[Hand-Finger-Gun]` | 指尖枪 | imitating pistol, pointing at camera/temple, with wink |

---

**A3. 甜蜜（Sweet）**

| 标签 | 姿态 | 关键词 |
|------|------|--------|
| `[Hand-Heart]` | 手比爱心 | forming heart shape, over chest/head/face |
| `[Hand-Blow-Kiss]` | 吹送飞吻 | palm touching lips, blowing kiss towards camera |
| `[Hand-Cup-Face]` | 双手捧脸 | palms on cheeks, paired with bright smile |

---

**A4. 治愈（Healing）**

| 标签 | 姿态 | 关键词 |
|------|------|--------|
| `[Hand-Palm-Sun]` | 手心向阳 | palm open towards sky, receiving sunlight/rain/breeze |
| `[Hand-On-Heart]` | 轻抚胸口 | one hand gently over heart, conveying peace/relief |
| `[Hand-Self-Hug]` | 自我拥抱 | arms wrapped around own shoulders/arms, self-comfort |
| `[Hand-Touch-Nature]` | 感受自然 | fingertips gently touching leaf, water surface, petal |

---

#### 分类B：内敛与中性情绪

**B1. 优雅（Elegant）**

| 标签 | 姿态 | 关键词 |
|------|------|--------|
| `[Hand-Ballet]` | 芭蕾手 | fingers extended with slight curve, wrist soft, on collarbone |
| `[Hand-Orchid]` | 兰花指 | delicately pinching skirt corner, teacup, page |
| `[Hand-Wrists-Cross]` | 手腕交叠 | hands gently crossed at wrists, front or lap |
| `[Hand-Support-Chin]` | 轻托下巴 | back of hand or curved fingers supporting chin side |

---

**B2. 温柔（Tender）**

| 标签 | 姿态 | 关键词 |
|------|------|--------|
| `[Hand-Tuck-Hair]` | 整理发丝 | gently tucking strand behind ear |
| `[Hand-Reach-Out]` | 伸出的手 | hand extended towards camera, palm slightly up, invitation |
| `[Hand-Loose-Grip]` | 虚握 | fingers lightly interlaced, not clenched, resting in lap |

---

**B3. 思考（Thinking）**

| 标签 | 姿态 | 关键词 |
|------|------|--------|
| `[Hand-Stroke-Chin]` | 摩挲下巴 | thumb and index finger gently holding/stroking chin |
| `[Hand-Temple]` | 手抵额头 | fingers pressed against temple, thoughtful |

---

#### 分类C：复杂与负面情绪

**C1. 忧郁（Melancholy）**

| 标签 | 姿态 | 关键词 |
|------|------|--------|
| `[Hand-Wipe-Tear]` | 手背拭泪 | back of hand brushing below eye |
| `[Hand-In-Hair]` | 抱头 | hands in hair, cradling back of head, body curled |
| `[Hand-Clutch-Arm]` | 紧抓手臂 | tightly gripping own arm/shoulder, self-comfort |
| `[Hand-Window]` | 指尖划过窗玻璃 | finger tracing line down glass window, separation |

---

**C2. 神秘（Mysterious）**

| 标签 | 姿态 | 关键词 |
|------|------|--------|
| `[Hand-Veil]` | 面纱手 | using hand/fingers to create slit over face, one eye visible |
| `[Hand-Cover-Lips]` | 遮蔽嘴唇 | fingers horizontally over lips, implying secret |
| `[Hand-Play-Props]` | 玩弄道具 | fiddling with tarot card, mask, key |

---

#### 分类D：强烈与攻击性情绪

**D1. 魅惑/诱惑（Alluring / Tempting）**

| 标签 | 姿态 | 关键词 |
|------|------|--------|
| `[Hand-Graze-Body]` | 指尖划过身体 | slowly tracing line along lips, neck, collarbone, thigh |
| `[Hand-Bite-Finger]` | 轻咬指尖 | gently placing tip of index/thumb between lips |
| `[Hand-Pull-Clothing]` | 拉扯衣物 | hooking finger on strap/collar, adjusting/removing gesture |
| `[Hand-Beckon]` | 勾手指 | index finger crooked in beckoning motion |
| `[Hand-Twirl-Hair]` | 把玩头发 | wrapping strand around finger |

---

**D2. 强大（Powerful）**

| 标签 | 姿态 | 关键词 |
|------|------|--------|
| `[Hand-Fist]` | 紧握拳头 | fist clenched tightly at side or in other hand |
| `[Hand-On-Hips]` | 双手叉腰 | hands on hips, authority and confidence |
| `[Hand-Arms-Cross]` | 双臂交叉 | arms folded across chest, defensive/resolute |

---

**D3. 傲慢/轻蔑（Arrogant / Scornful）**

| 标签 | 姿态 | 关键词 |
|------|------|--------|
| `[Hand-Inspect-Nails]` | 端详指甲 | lifting hand to inspect fingernails casually, disdain |
| `[Hand-Flick-Dust]` | 弹灰动作 | flicking non-existent dust from shoulder |
| `[Hand-Stop]` | "停止"手势 | holding palm out towards viewer |
| `[Hand-Point-Arrogant]` | 指点 | pointing with index finger, head held high, looking away |

---

#### 分类E：主干道专属姿态

**E1. 高级时尚奇观（Pillar A）**

| 标签 | 姿态 | 关键词 |
|------|------|--------|
| `[Hand-Geometric]` | 建筑感手型 | fingers creating sharp geometric angles |
| `[Hand-Frame]` | 构成框架 | hands forming deliberate frame within image |
| `[Hand-Light-Play]` | 与光互动 | palm catching light beam, light through fingers |
| `[Hand-Voguing]` | Voguing舞姿 | sharp angles, fast-motion implied, dance-inspired |

---

**E2. 生活叙事温度（Pillar B）**

| 标签 | 姿态 | 关键词 |
|------|------|--------|
| `[Hand-Adjust-Cuff]` | 整理袖口 | adjusting cuffs, natural gesture |
| `[Hand-Tie-Shoe]` | 系鞋带 | tying shoelaces, casual |
| `[Hand-Fiddle-Necklace]` | 无意识拨弄项链 | unconsciously fiddling with necklace |
| `[Hand-In-Pocket]` | 单手插口袋 | one hand casually in pocket |
| `[Hand-On-Lap]` | 双手放膝 | hands resting softly on lap |

---

### 5.1.4 腿部姿态与构图

#### A. 通用构图

**坐姿（Seated）**

| 标签 | 姿态 | 关键词 |
|------|------|--------|
| `[Leg-Sit-Stool]` | 高脚凳坐姿 | sitting on high stool, legs crossed or extending forward |
| `[Leg-Sit-Stairs]` | 台阶坐 | sitting on stairs/platform, casual |
| `[Leg-Sit-Sofa]` | 沙发慵懒坐 | lazy sofa sit, relaxed, sprawled |
| `[Leg-Sit-Knee-Hug]` | 抱膝坐 | knee-hug sit, arms around knees |

---

**蹲/跪姿（Crouching / Kneeling）**

| 标签 | 姿态 | 关键词 |
|------|------|--------|
| `[Leg-Squat-Street]` | 街头风蹲姿 | street-style squat, urban |
| `[Leg-Kneel-One]` | 单膝跪 | one-knee kneel, elegant or warrior-like |
| `[Leg-Kneel-Side]` | 侧跪坐 | side-knee sit, traditional, feminine |

---

**站姿（Standing）**

| 标签 | 姿态 | 关键词 |
|------|------|--------|
| `[Leg-Stand-Lean]` | 倚靠站姿 | leaning against wall/car, casual |
| `[Leg-Stand-One-Leg]` | 单腿站立/抬腿 | one-legged stand, leg lift, dynamic |
| `[Leg-Stand-Height]` | 利用高低差 | using stairs/platform for height difference |

---

#### B. 主干道A：时尚奇观

**动态姿态**

| 标签 | 姿态 | 关键词 |
|------|------|--------|
| `[Leg-Walk-Mid]` | 迈步中 | mid-stride, walking pose, motion |
| `[Leg-Twirl]` | 轻柔旋转 | gentle twirl/spin, skirt flowing |
| `[Leg-Catwalk]` | 猫步前行 | catwalk strut, confident |

---

**不对称与建筑感**

| 标签 | 姿态 | 关键词 |
|------|------|--------|
| `[Leg-Lift-High]` | 单腿高抬 | high leg lift, dramatic, ballet-like |
| `[Leg-Power-Stance]` | 夸张力量站姿 | exaggerated power stance, legs wide |
| `[Leg-Spread-Chair]` | 椅上双腿大开 | legs spread on chair, dominant |

---

#### C. 主干道B：生活叙事

**自然站姿**

| 标签 | 姿态 | 关键词 |
|------|------|--------|
| `[Leg-Contrapposto]` | 稍息站姿 | contrapposto, weight shifted to one leg, relaxed |
| `[Leg-Planted]` | 双脚稳稳站立 | firmly planted, grounded |
| `[Leg-Ankles-Cross]` | 脚踝处交叉 | ankles casually crossed |

---

**情境化坐姿**

| 标签 | 姿态 | 关键词 |
|------|------|--------|
| `[Leg-Sit-Steps]` | 坐在台阶 | sitting on steps, casual, waiting |
| `[Leg-Slouch-Couch]` | 窝在沙发 | slouching on couch, relaxed |
| `[Leg-Cross-Floor]` | 盘腿坐地 | cross-legged on floor, informal |
| `[Leg-Sit-Desk]` | 坐书桌边缘 | sitting on edge of desk |

---

## 5.2 互动叙事（Interactive Narrative）

### 5.2.1 激活条件

**何时使用互动模块：**
- 单个角色不足以承载叙事深度
- 需要展现关系动态
- 创造更复杂的情感层次

---

### 5.2.2 与人类互动（Human Interaction）

#### 步骤1：定义关系

| 标签 | 关系 | 说明 |
|------|------|------|
| `[Interact-Sisters]` | 姐妹 | 血缘、亲密、互相扶持 |
| `[Interact-Friends]` | 挚友 | 深厚友谊、分享秘密 |
| `[Interact-Rivals]` | 对手 | 竞争、对立、张力 |
| `[Interact-Mirror]` | 镜像自我 | 自我对话、双重性格 |
| `[Interact-Strangers]` | 陌生人 | 初遇、距离感、好奇 |

---

#### 步骤2：定义互动模式

**协作式（Collaborative）**

| 标签 | 互动 | 关键词 |
|------|------|--------|
| `[Interact-Joint-Activity]` | 共同活动 | painting together, cooking together, studying map |

---

**亲密与玩闹（Intimacy & Playfulness）**

| 标签 | 互动 | 关键词 |
|------|------|--------|
| `[Interact-Whisper]` | 耳语 | whispering secrets, leaning close |
| `[Interact-Hug]` | 温暖拥抱 | warm embrace, gentle hug from behind |
| `[Interact-Playful]` | 嬉戏打闹 | playful antics, piggyback ride, pillow fight, splashing water |
| `[Interact-Shared-Moment]` | 共享瞬间 | sharing headphones, leaning on shoulder while reading |

---

**对比动态（Contrasting Dynamics）**

| 标签 | 互动 | 关键词 |
|------|------|--------|
| `[Interact-Emotion-Contrast]` | 情绪对比 | one smiling, one looking away; one sitting, one dancing |

---

**保护姿态（Protective）**

| 标签 | 互动 | 关键词 |
|------|------|--------|
| `[Interact-Care]` | 温柔照顾 | wiping tears, smoothing hair, watching over |

---

#### 步骤3：互补人设（可选）

**气质对比：**
- lively and cheerful vs. serene and elegant
- passionate and bold vs. aloof and distant

**风格对比：**
- ethereal in white vs. gothic in black lace
- qipao-clad with old-world charm vs. streetwear-clad and urban

**角色对比：**
- older-sister energy vs. clingy and trusting
- commanding and intense vs. demure and shy

---

#### 主干道专属互动

**A. 时尚奇观（Pillar A）**

| 标签 | 互动 | 关键词 |
|------|------|--------|
| `[Interact-Back-to-Back]` | 背对背 | back-to-back, stylized formation |
| `[Interact-Geometric]` | 几何队形 | forming geometric shapes with limbs |
| `[Interact-Almost-Kiss]` | 将吻未吻 | the almost kiss, dramatic tension |
| `[Interact-Gaze-Apart]` | 望向不同方向 | gazing in different directions |

---

**B. 生活叙事（Pillar B）**

| 标签 | 互动 | 关键词 |
|------|------|--------|
| `[Interact-Point-Out]` | 指出远方 | pointing something out in distance |
| `[Interact-Tie-Shoe]` | 为对方系鞋带 | one tying other's shoelace |
| `[Interact-Lean]` | 身体倚靠 | bodies leaning against each other while seated |
| `[Interact-Hand-Rest]` | 手放肩膀/后腰 | hand resting on shoulder/lower back |

---

### 5.2.3 与动物互动（Animal Interaction）

#### 步骤1：选择生物（完整列表）

**林地、草原与灌木丛：**
- 鹿/羚羊（Deer/Antelope）
- 狐狸/芬狐（Fox/Fennec Fox）
- 兔子/野兔（Rabbit/Hare）
- 松鼠（Squirrel）
- 浣熊（Raccoon）
- 熊（Bear）
- 长颈鹿（Giraffe）
- 斑马（Zebra）
- 大象（Elephant）

**山地、雪原：**
- 狼（Wolf）
- 雪豹（Snow Leopard）
- 猞猁（Lynx）
- 北极熊（Polar Bear）
- 北极狐（Arctic Fox）
- 驯鹿（Reindeer）

**热带、丛林：**
- 老虎/白虎（Tiger/White Tiger）
- 狮子/白狮（Lion/White Lion）
- 豹/黑豹（Leopard/Panther）
- 猴子（Monkey）
- 树懒（Sloth）
- 熊猫（Panda）
- 小熊猫（Red Panda）
- 羊驼（Alpaca）
- 水豚（Capybara）

**鸟类：**
- 鹰（Eagle）
- 隼（Falcon）
- 猫头鹰（Owl）
- 天鹅（Swan）
- 鹤（Crane）
- 鸳鸯（Mandarin Duck）
- 火烈鸟（Flamingo）
- 孔雀（Peacock）
- 鹦鹉（Parrot）
- 蜂鸟（Hummingbird）

**海洋、河流：**
- 海豚/虎鲸（Dolphin/Orca）
- 海龟（Sea Turtle）
- 海豹（Seal）
- 水獭（Otter）
- 锦鲤（Koi Fish）

**伴侣型：**
- 猫（Cat）- 可指定品种（Ragdoll, Maine Coon）
- 狗（Dog）- 可指定品种（Shiba Inu, Samoyed）
- 仓鼠/龙猫（Hamster/Chinchilla）

**🟡 TERP提醒**：
- 狐狸是"显性元素"，避免过度使用
- 主动探索"微妙"动物（如：鹤、鹿、蝴蝶、水獭）

**⚠️ 绝对禁止**：
- ❌ 蜘蛛（Spider）
- ❌ 蝙蝠（Bat）
- ❌ 蛇（Snake）- 除非引擎A超现实并置
- ❌ 老鼠（Rat）

---

#### 步骤2：定义互动动态

**温柔联结（Gentle Bonding）**

| 标签 | 互动 | 关键词 |
|------|------|--------|
| `[Animal-Stroke]` | 轻柔抚摸 | soft strokes, gentle petting |
| `[Animal-Nuzzle]` | 相互蹭脸 | nuzzling, affectionate touch |
| `[Animal-Feed]` | 喂食 | offering food, hand-feeding |

---

**志趣相投（Kindred Spirits）**

| 标签 | 互动 | 关键词 |
|------|------|--------|
| `[Animal-Side-by-Side]` | 并肩而立 | side by side, companionship |
| `[Animal-Gaze-Together]` | 共同眺望 | gazing at horizon together |

---

**胆怯好奇（Timid Curiosity）**

| 标签 | 互动 | 关键词 |
|------|------|--------|
| `[Animal-Tentative]` | 试探性接触 | tentative steps, cautious approach |
| `[Animal-Eye-Lock]` | 锁定眼神 | locked eyes, mutual curiosity |

---

#### 主干道专属互动

**A. 时尚奇观（Pillar A）**

| 标签 | 互动 | 关键词 |
|------|------|--------|
| `[Animal-Surreal]` | 超现实并置 | snake coiled around arm (遵守美学前提) |
| `[Animal-Pattern-Echo]` | 图案呼应 | zebra stripes echoing dress pattern |
| `[Animal-Exotic-Pose]` | 异域鸟类姿态 | elegant pose with peacock/macaw |

---

**B. 生活叙事（Pillar B）**

| 标签 | 互动 | 关键词 |
|------|------|--------|
| `[Animal-Pet-Greet]` | 宠物迎接 | pet greeting excitedly at door |
| `[Animal-Walk-Dog]` | 遛狗 | taking dog for walk in park |
| `[Animal-Pet-Family]` | 动物作为家庭成员 | dog sitting at dinner table, cat napping on laundry |
| `[Animal-Working]` | 工作中的动物 | shepherd with sheepdog, farmer with livestock |

---

#### 特殊：猛兽驯化（Apex Predator Domestication）

**⚠️ 重要规则：**

**适用对象：**
- 狮子、老虎、豹子、狼、熊等顶级掠食者

**互动逻辑：**
- 必须打破"恐惧"常规
- 角色表现绝对主宰感（Dominance）或家庭般亲昵（Familial Intimacy）
- 严禁表现出恐惧或对峙

**示例关键词：**
```
stroking a panther as if it were a house cat
casually leaning against a lion
walking a wolf on a leash like a pet dog
playing with a tiger cub
```

---

## 📊 姿态系统快速决策树

```
确定场景与角色情绪
    ↓
单人姿态 还是 互动叙事？
    ↓
┌─────────────────────┬─────────────────────┐
│   单人姿态           │   互动叙事           │
├─────────────────────┼─────────────────────┤
│ 1. 选择手部姿态     │ 1. 选择互动类型     │
│    （情绪匹配）     │    （人物/动物）    │
│ 2. 选择腿部姿态     │ 2. 定义关系         │
│    （站/坐/蹲）     │ 3. 定义互动模式     │
│ 3. 确定视角         │ 4. 可选：互补人设   │
│    （正面/侧面）    │                     │
│ 4. 背视回眸（如需） │                     │
└─────────────────────┴─────────────────────┘
    ↓
与局部美学焦点联动
    ↓
确保姿态自然且符合场景逻辑
    ↓
完成姿态描述
```

---

## 🎯 姿态系统使用提示

### 1. 情绪与姿态匹配
```
✅ 正确：
"甜蜜浪漫场景" → 手比爱心、吹送飞吻
"忧郁孤独场景" → 抱头、手背拭泪

❌ 错误：
"悲伤场景" → 手比爱心（情绪不符）
```

---

### 2. 避免姿态堆砌
```
❌ 过度：
"She makes cat paws, blows a kiss, does a heart sign, and salutes"

✅ 精选：
"She makes a heart shape with her hands over her chest, smiling warmly"
```

---

### 3. 背视必须回眸
```
❌ 错误：
"back view, showing only the back of her head"

✅ 正确：
"back view, looking back over her shoulder with a gentle smile, 
revealing her side profile"
```

---

## 结语

场景与姿态系统是叙事的"载体"和"动作"。合理组合可以创造：
- **空间深度**：通过分层构图和氛围填充
- **情感表达**：通过手部姿态和面部表情
- **关系动态**：通过互动叙事和角色对比

下一步：VIBE引擎系统的重组优化（最后一部分）。
