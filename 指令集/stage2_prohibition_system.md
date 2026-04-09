# 阶段二：禁令系统优化（v2.0）

---

## 🎯 禁令系统设计哲学

**核心原则**：分级管理 + 快速检索 + 情境豁免

原指令集的问题：
- Level 1/Level 2 边界模糊
- 72+ 条禁令混在附录X，难以查找
- 豁免条件不清晰（"为服务特定创意"太主观）

优化方案：
- 🔴🟡🟢 三色分级，视觉化优先级
- 按功能分类（技术/内容/风格），而非堆砌
- 明确豁免触发条件 + 示例

---

## 🔴 第一级：绝对禁令（NEVER VIOLATE）

**适用范围**：所有情况，无例外，无豁免

**违反后果**：导致图像生成失败、内容审核不通过、或破坏模型稳定性

---

### 分类A：技术稳定性

#### A1. 渲染引擎术语
**禁止使用：**
- ❌ Unreal Engine 5 render
- ❌ V-Ray render  
- ❌ Octane Render
- ❌ Blender Cycles
- ❌ Arnold Renderer
- ❌ 任何3D渲染软件名称

**原因**：这些术语会触发AI生成3D渲染风格，破坏"超写实照片"基调

**替代方案**：
- ✅ cinematic lighting
- ✅ photorealistic
- ✅ hyperdetailed
- ✅ studio photography
- ✅ professional DSLR shot

---

#### A2. 镜头距离限制
**禁止使用：**
- ❌ long shot
- ❌ extreme long shot
- ❌ wide shot（如果指全景远景）
- ❌ aerial view / bird's eye view（如果距离过远）

**原因**：远景镜头会导致面部细节崩坏、特征扭曲

**允许使用：**
- ✅ close-up（特写）
- ✅ medium close-up（中特写）
- ✅ medium shot（中景）
- ✅ full shot（全景，但人物仍占画面主体）

**判断标准**：人物面部特征必须清晰可辨

---

#### A3. 元指令（Meta-Instructions）
**禁止使用：**
- ❌ shot on RED camera
- ❌ filmed with Arri Alexa
- ❌ captured on 35mm film
- ❌ film still from...
- ❌ live-action adaptation of...
- ❌ behind-the-scenes photo

**原因**：这些是"拍摄过程"描述，会混淆AI理解最终画面

**替代方案**：
- ✅ 直接描述画面效果：cinematic film grain, shallow depth of field

---

### 分类B：内容安全性

#### B1. 生物/解剖学异常
**绝对禁止：**
- ❌ horns（角）
- ❌ wings（翅膀）
- ❌ tails（尾巴）
- ❌ animal ears on humans（兽耳）
- ❌ extra limbs（多余肢体）
- ❌ 任何违反基本人体结构的特征

**特别注意**：
- 精灵耳（elf ears）：禁止
- 吸血鬼獠牙（vampire fangs）：禁止
- 即使是"幻想风格"也不允许

**原因**：违反"高度写实照片"基调，且可能触发内容审核

---

#### B2. 不适/恐怖元素
**绝对禁止：**
- ❌ corpses（尸体）
- ❌ skeletons（骷髅）
- ❌ blood（血液）
- ❌ wounds / injuries（伤口/受伤）
- ❌ bandages（绷带，除非时尚配饰用途）
- ❌ spiders（蜘蛛）
- ❌ spider webs（蜘蛛网）
- ❌ bats（蝙蝠）
- ❌ snakes（蛇）
- ❌ rats（老鼠）

**氛围禁令：**
- ❌ horror atmosphere（恐怖氛围）
- ❌ dark and disturbing（黑暗压抑）
- ❌ eerie / creepy（诡异）
- ❌ abandoned hospital / asylum（废弃医院/精神病院）

**原因**：负面情绪内容，违反"积极美学"原则

---

#### B3. 医疗/治疗场景
**绝对禁止：**
- ❌ veterinarian（兽医场景）
- ❌ treating injuries（治疗伤口）
- ❌ medical examination（医学检查）
- ❌ hospital bed（病床）
- ❌ IV drip（输液）
- ❌ surgical tools（手术器械）

**原因**：容易产生不适联想

---

#### B4. 密集恐惧症触发器
**绝对禁止：**
- ❌ honeycomb patterns（蜂巢图案）
- ❌ lotus seed pod（莲蓬）
- ❌ dense repetitive holes（密集重复孔洞）
- ❌ barnacles（藤壶）
- ❌ 任何可能引发密集恐惧症的纹理

**原因**：生理不适反应

---

### 分类C：服装与身体规范

#### C1. 内衣展示限制
**绝对禁止：**
- ❌ bras / bra sets 作为独立展示的主体
- ❌ corsets（紧身胸衣）
- ❌ bustiers（束腹）
- ❌ underwear as outerwear（内衣外穿，除非是时尚设计的吊带背心）

**允许的边缘情况：**
- ✅ 抹胸式礼服（strapless gown）- 这是外衣
- ✅ 吊带背心（camisole）作为外穿上衣 - 但必须是时尚设计，非内衣款式
- ✅ 运动内衣（sports bra）若与运动外套搭配

**判断标准**：是否明显是"内衣"范畴

---

#### C2. 材质限制
**绝对禁止：**
- ❌ latex clothing（乳胶材质服装）
- ❌ vinyl clothing（乙烯基材质）
- ❌ PVC clothing（PVC材质）
- ❌ rubber clothing（橡胶材质）

**原因**：这些材质强烈关联特定亚文化，不符合主流美学定位

---

#### C2.5 连体服禁令（重要）
**绝对禁止：**
- ❌ jumpsuit（连体裤）
- ❌ catsuit（紧身连体衣）
- ❌ bodysuit as complete outfit（紧身全身衣作为完整穿搭）
- ❌ full-body suit / one-piece body suit（全身连体服）
- ❌ unitard（连体紧身衣）

**无论以何种风格包装均不可用，包括但不限于：**
- ❌ 以"未来感"/"高科技"为由使用
- ❌ 以"运动风格"为由使用（运动背心+短裤可替代）
- ❌ 以"极简美学"为由使用

**原因**：连体服将人物包裹为单一色块，严重破坏服装与身体的层次叙事，削弱视觉细节密度

**替代方案：**
- ✅ 想要未来感 → 高领修身针织 + 皮质阔腿裤 + 金属腰带
- ✅ 想要运动感 → 运动背心 + 运动短裤/紧身裤 + 外搭
- ✅ 想要极简感 → 真丝吊带裙 + 剪裁精良外套

---

#### C3. 身体描述规范
**绝对禁止：**
- ❌ plus-size body type（大码身材）
- ❌ 使用 "breast" 一词

**必须使用的优雅措辞：**
- ✅ slender figure（纤细身材）
- ✅ graceful physique（优雅体态）
- ✅ delicate frame（精致骨架）
- ✅ 描述服装贴合度：fitted bodice, form-fitting silhouette

**原因**：保持高级时尚美学标准 + 避免敏感词

---

### 分类D：场景与世界观限制

#### D1. 科幻/未来主义
**绝对禁止：**
- ❌ Cyberpunk（赛博朋克）
- ❌ Steampunk（蒸汽朋克）
- ❌ space station（太空站）
- ❌ alien planet（外星球）
- ❌ holographic displays（全息显示）
- ❌ flying cars（飞行汽车）
- ❌ robot / android（机器人/人造人）
- ❌ laser weapons（激光武器）

**原因**：超出"当前世界已知科技水平"，违反写实基调

**允许的科技元素：**
- ✅ 现代都市霓虹灯
- ✅ 当代电子设备（手机、平板、LED屏幕）
- ✅ 摩登建筑设计

---

#### D2. 生物发光/超自然
**绝对禁止：**
- ❌ bio-luminescence（生物发光）
- ❌ glowing mushrooms（发光蘑菇）
- ❌ bioluminescent plants（发光植物）
- ❌ glowing creatures（发光生物）
- ❌ 任何"幻想生态"元素

**原因**：不存在于地球真实生态系统

**允许的发光效果：**
- ✅ 人工光源：neon lights, LED strips, lanterns
- ✅ 自然光学现象：fireflies（萤火虫，真实存在）

---

#### D3. 极端尺度
**绝对禁止：**
- ❌ 微观尺度：cells, molecules, atoms
- ❌ 宇宙尺度：galaxies, nebulae, black holes
- ❌ "咖啡杯里的星云"等超现实概念

**原因**：人类感知尺度之外，违反写实原则

---

#### D4. 特定场景类型
**绝对禁止：**
- ❌ bio-labs（生物实验室）
- ❌ control rooms（控制室）
- ❌ cockpits（驾驶舱）
- ❌ scenes centered on sculptures（以雕塑作品为核心）
- ❌ table covered in many small objects（桌上堆满杂物）

**原因**：
- 实验室：容易产生不适/冷冰冰的联想
- 控制室/驾驶舱：技术复杂度高，AI难以准确生成
- 雕塑为核心：抢夺人物主体地位
- 杂物堆：视觉混乱，破坏构图

---

### 分类E：姿态与行为

#### E1. 背面姿态限制
**绝对禁止：**
- ❌ 完全背对镜头只露后脑勺（back of head only）

**允许的背面姿态：**
- ✅ over-the-shoulder view（过肩视角，能看到侧脸）
- ✅ three-quarter back view（四分之三背面，能看到部分面部轮廓）
- ✅ looking back pose（回眸姿态）

**原因**：完全看不到脸会失去表情细节，降低吸引力

---

#### E2. 物理违反
**绝对禁止：**
- ❌ levitating / floating（无故悬浮）
- ❌ defying gravity（违反重力）
- ❌ impossible poses（不可能的姿势）

**原因**：破坏写实感

---

## 🟡 第二级：风格规避（有条件豁免）

**适用范围**：默认应避免，但在特定创意需求下可豁免

**豁免条件**：
1. 服务于"生活叙事温度"主题（市井、职场、运动等日常场景）
2. 或用于"反常规组合"创意（如华丽服饰 + 简陋环境的反差）
3. 且豁免不违反🔴第一级任何禁令
4. 且必须导向"美观"或"有趣"的视觉效果，而非"廉价"或"粗糙"

---

### 分类A：服装面料

**建议避免：**
- 🟡 tattered cloth（破旧布料）
- 🟡 frayed edges（磨损边缘）
- 🟡 faded colors（褪色）
- 🟡 cheap-looking fabrics（廉价感面料）
- 🟡 rough textures（粗糙质地）

**豁免示例：**
```
❌ 无意义使用：
"她穿着破旧的T恤在豪华酒店" - 不协调且无创意

✅ 有意义豁免：
"她穿着洗旧的牛仔夹克和复古T恤，坐在老式唱片店的木凳上，
翻看着泛黄的黑胶唱片封套" - 服务于怀旧/市井叙事
```

---

### 分类B：服装款式

#### B1. 高领类
**建议避免：**
- 🟡 turtlenecks（高领毛衣）
- 🟡 mock necks（半高领）
- 🟡 bulky knitwear（笨重针织品）

**例外：**
- ✅ Mandarin collar（旗袍立领）- 永远允许

**豁免示例：**
```
✅ 冬季都市叙事：
"她穿着米色高领羊绒衫，外搭长款大衣，双手捧着热咖啡，
站在飘雪的街角，蒸汽从杯口升起模糊了眼镜"
- 服务于季节真实感和温暖氛围
```

---

#### B2. 腿部着装
**建议避免：**
- 🟡 stockings（长筒袜）
- 🟡 pantyhose（裤袜）
- 🟡 tights（紧身裤袜）
- 🟡 fishnets（网袜）

**豁免示例：**
```
✅ 职场OL风格：
"她穿着黑色修身职业套裙，肉色裤袜，黑色尖头高跟鞋，
站在落地窗前的办公桌旁翻阅文件，窗外是都市夜景"
- OL制服的标准组成部分
```

---

#### B3. 盔甲类
**建议避免：**
- 🟡 heavy armor（重甲）
- 🟡 full plate armor（全身板甲）
- 🟡 chainmail（锁子甲）

**允许：**
- ✅ 风格化轻甲（streamlined light armor with elegant lines）
- ✅ 仪式性/幻想盔甲（ceremonial armor, fantasy-styled with graceful design）

**判断标准**：是否具有美学线条，而非纯功能性厚重感

---

### 分类C：设计简约度

**建议避免：**
- 🟡 overly minimalist clothing（过于简约的服装）
- 🟡 plain solid color with no details（纯色无细节）

**原因**：缺乏视觉兴趣点

**豁免条件**：
- 通过其他元素补偿（复杂场景、戏剧化光影、精致妆容）
- 或故意追求极简美学（需搭配高级材质）

**豁免示例：**
```
✅ 极简 + 复杂环境：
"她穿着纯白色简约吊带裙，站在繁复的巴洛克镜厅中，
无数镜面反射形成无限空间"
- 服装简约反衬环境复杂度

✅ 极简 + 材质升级：
"她穿着剪裁精良的炭灰色真丝slip dress，
丝绸表面随身体曲线流动，微妙的光泽变化"
- 简约但有高级质感
```

---

## 🟢 第三级：创意优化建议（非强制）

**性质**：提升质量的最佳实践，但不违反也不会导致失败

---

### A. 组合多样性

**建议：**
- 🟢 避免过度依赖"显性元素"（哥特、苗疆、狐狸等）
- 🟢 每批创意中，同一元素不超过2-3次
- 🟢 主动探索"微妙"元素（宋制汉服、洛可可、兔子等）

**自检方法：**
```
生成20个概念后，统计：
- "哥特"出现几次？> 2次 → 需要替换
- "废墟"出现几次？> 3次 → 需要换场景
- 动物种类是否单一？只有狐狸和猫 → 增加鹿、鹤、蝴蝶
```

---

### B. 细节密度

**建议：**
- 🟢 每条描述融合 5-7 个不同维度的元素
- 🟢 避免"空虚"背景（纯色背景、无限虚空）
- 🟢 强制使用前景-中景-背景分层

**负面示例：**
```
❌ 低密度：
"一个女孩穿着白裙站在草地上"
- 只有3个元素：人物+服装+场景

✅ 高密度：
"Close-up of a young woman with long black hair in a loose braid, 
wearing an ivory linen sundress with lace trim, standing in a 
wildflower meadow. Foreground: out-of-focus purple lupines. 
Background: distant birch forest. Golden hour side lighting, 
shallow depth of field."
- 包含：发型、服装、场景、前景、背景、光影、景深
```

---

### C. 反常规组合

**建议：**
- 🟢 尝试"意外组合"提升创意
- 🟢 打破固定搭配（哥特+废墟、汉服+古建筑）

**创意公式：**
```
[高雅元素] + [低俗/日常场景] = 反差美学
[传统文化] + [现代都市] = 时空交错
[运动休闲] + [宫殿] = 身份错位
```

**示例：**
```
🟢 洛可可洋装 + 工业废墟 + 钢琴
🟢 运动背心短裤 + 欧式图书馆 + 古籍
🟢 汉服 + 霓虹都市 + 摩托车
🟢 婚纱 + 荒漠戈壁 + 骆驼
```

---

## 📋 快速自检清单（生成前使用）

### 第一遍：内容安全扫描（🔴级）

```
☐ 没有3D渲染术语（Unreal Engine等）
☐ 没有远景镜头（long shot等）
☐ 没有生物异常（角、翅膀、兽耳等）
☐ 没有恐怖元素（血液、骷髅、蜘蛛等）
☐ 没有医疗场景（治疗、绷带、兽医等）
☐ 没有禁忌服装（胸罩、紧身胸衣、乳胶、连体衣/jumpsuit等）
☐ 没有科幻元素（赛博朋克、太空、全息等）
☐ 没有生物发光（发光蘑菇、发光植物等）
☐ 没有违反物理定律（悬浮、违反重力等）
☐ 没有使用"breast"一词
```

### 第二遍：术语纯净度检查（🔴级）

```
☐ 没有出现内部术语（VIBE、引擎、解耦、凝固瞬息等）
☐ 没有出现导演/艺术家名字（新海诚、王家卫等）
☐ 没有出现括号或方括号 ( ) [ ]
☐ 没有出现编号（0.0.1、P-001等）
☐ 没有出现引号引用术语（"decoupling"等）
```

### 第三遍：质量优化检查（🟢级）

```
☐ 是否以技术前缀开头（masterpiece, best quality...）
☐ 字数是否达到900+字符
☐ 是否包含前景-中景-背景分层
☐ 是否避免了显性元素重复（哥特、苗疆<3次）
☐ 是否包含具体的光影描述
☐ 中文部分是否采用流动叙事而非清单
```

---

## 🔍 豁免决策流程图

```
需要使用🟡级禁令中的元素？
    ↓
    问题1：是否服务于以下任一目的？
    - [ ] 生活叙事温度（市井、日常、真实感）
    - [ ] 反常规组合（创造视觉反差）
    - [ ] 季节/天气真实性（如冬天的毛衣）
    ↓
    如果否 → ❌ 不使用，选择其他元素
    ↓
    如果是 → 继续问题2
    ↓
    问题2：这个使用是否违反任何🔴级禁令？
    ↓
    如果是 → ❌ 绝对不可使用
    ↓
    如果否 → 继续问题3
    ↓
    问题3：最终效果是否导向"美观"或"有趣"？
    ↓
    如果否（廉价、粗糙、不适）→ ❌ 不使用
    ↓
    如果是 → ✅ 豁免批准，可以使用
```

---

## 📚 禁令速查表（按字母排序）

| 禁用内容 | 级别 | 可否豁免 |
|---------|------|---------|
| abandoned hospital | 🔴 | 否 |
| aerial view | 🔴 | 否 |
| animal ears | 🔴 | 否 |
| bandages | 🔴 | 否（除非纯装饰） |
| bats | 🔴 | 否 |
| bio-labs | 🔴 | 否 |
| bio-luminescence | 🔴 | 否 |
| blood | 🔴 | 否 |
| bras / bra sets | 🔴 | 否 |
| breast (词汇) | 🔴 | 否 |
| bustiers | 🔴 | 否 |
| corsets | 🔴 | 否 |
| corpses | 🔴 | 否 |
| Cyberpunk | 🔴 | 否 |
| extreme long shot | 🔴 | 否 |
| fishnets | 🟡 | 可（OL风格） |
| heavy armor | 🟡 | 可（仪式性轻甲） |
| holographic | 🔴 | 否 |
| honeycomb patterns | 🔴 | 否 |
| horns | 🔴 | 否 |
| latex clothing | 🔴 | 否 |
| levitating | 🔴 | 否 |
| long shot | 🔴 | 否 |
| lotus seed pod | 🔴 | 否 |
| mushroom (发光) | 🔴 | 否 |
| Octane Render | 🔴 | 否 |
| pantyhose | 🟡 | 可（职场） |
| plus-size | 🔴 | 否 |
| skeletons | 🔴 | 否 |
| snakes | 🔴 | 否 |
| space station | 🔴 | 否 |
| spiders | 🔴 | 否 |
| Steampunk | 🔴 | 否 |
| tattered cloth | 🟡 | 可（怀旧叙事） |
| turtlenecks | 🟡 | 可（冬季场景） |
| Unreal Engine | 🔴 | 否 |
| veterinarian | 🔴 | 否 |
| vinyl clothing | 🔴 | 否 |
| wings | 🔴 | 否 |
| wounds | 🔴 | 否 |

---

## 🎓 常见误区与正确做法

### 误区1：过度简化
```
❌ 错误思路：
"禁令太多记不住，我就写简单点，减少元素"

✅ 正确做法：
使用自检清单系统化检查，而非削减创意
```

### 误区2：机械规避
```
❌ 错误思路：
"因为丝袜是🟡级，所以我永远不用"

✅ 正确做法：
理解禁令背后的原因（避免低俗感），在合适情境豁免
（如职场OL风格）
```

### 误区3：忽视分级
```
❌ 错误思路：
"都是禁令，都一样重要"

✅ 正确做法：
🔴级绝不违反，🟡级根据情境判断，🟢级作为优化参考
```

---

## 💡 实战案例

### 案例1：科幻元素的正确处理

**用户需求**："未来感的都市场景"

**❌ 错误做法：**
```
"Cyberpunk cityscape with holographic billboards and flying cars..."
- 违反🔴级禁令：Cyberpunk, holographic, flying cars
```

**✅ 正确做法：**
```
"Modern metropolitan skyline at night, towering glass skyscrapers 
with LED facade lighting displaying colorful geometric patterns, 
sleek contemporary architecture with reflective surfaces, 
bustling street below with neon signs and modern vehicles, 
high-tech aesthetic within current technology bounds..."
- 保留未来感，但使用现有科技（LED、现代建筑）
```

---

### 案例2：破旧元素的豁免使用

**用户需求**："怀旧复古的唱片店场景"

**❌ 无脑规避：**
```
"穿着崭新的华丽洋装在古董唱片店"
- 服装与场景不协调
```

**✅ 合理豁免：**
```
"She wears a vintage washed denim jacket with faded patches, 
a soft worn-in band t-shirt, and distressed jeans. She sits 
on a wooden stool in a retro vinyl record shop, flipping 
through aged album covers with yellowed edges..."
- 🟡级豁免：tattered/faded 服务于怀旧叙事
- 所有元素协调一致
```

---

### 案例3：极简服装的补偿策略

**用户需求**："简约时尚风格"

**❌ 单纯简约：**
```
"plain white t-shirt and black pants in a white room"
- 过于简约 + 空虚背景 = 无趣
```

**✅ 补偿策略：**
```
"She wears a perfectly tailored white silk blouse with subtle 
sheen and minimalist black wide-leg trousers. She stands in a 
brutalist concrete corridor with dramatic angular shadows cast 
by skylights above. Geometric light patterns on the textured 
walls. High contrast black and white aesthetic with architectural 
complexity compensating for clothing simplicity."
- 简约服装 + 复杂建筑光影 = 平衡
```

---

## 📖 术语翻译参考

**用于理解原始指令集术语**

| 原术语 | 新表述 | 在禁令中的位置 |
|--------|--------|---------------|
| Level 1 绝对禁止 | 🔴 第一级 | 永不违反 |
| Level 2 风格规避 | 🟡 第二级 | 可豁免 |
| 高级时尚奇观 | - | 🟡豁免条件参考 |
| 生活叙事温度 | - | 🟡豁免条件之一 |
| 解耦原则 | 反常规组合 | 🟡豁免条件之一 |
| 积极美学SOP | 美观/壮观导向 | 豁免决策问题3 |

---

## 结语

**禁令的本质**：不是限制创意，而是确保创意在"可实现"和"高质量"的边界内。

**使用建议**：
1. 生成前：扫描🔴级清单（10秒）
2. 生成后：完整自检（30秒）
3. 不确定时：参考案例和决策流程图

**记住**：🔴级是红线，🟡级是弹性，🟢级是追求。
