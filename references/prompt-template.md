# 生图提示词模板

每张图单独生成。根据正文内容替换变量，不要把多张图拼在一起。

```text
Generate one standalone 16:9 horizontal Chinese article comic illustration.

Visual DNA:
Pure white background. Minimalist black hand-drawn line art. Slightly wobbly pen lines. Lots of empty white space. Sparse red/orange/blue handwritten Chinese annotations. Clean absurd product-sketch feeling. No gradients, no shadows, no paper texture, no complex background, no commercial vector style, no PPT infographic look, no cute mascot poster, no children's illustration, no realistic UI.

Recurring IP character required:
夜航猫头鹰, a colored owl operator, not black. Warm ochre/orange face disk and ear tufts, muted teal-blue head/body, oversized black sunglasses, deep blue loose robe, plain white coffee mug, thin simple legs, blank deadpan expression. It must perform the core conceptual action, not decorate the scene. Use the mood and complexity of assets/nightsailing-owl-reference.png: recognizable, hand-drawn, restrained, not overly simplified unless requested.

Important content isolation:
NightSailing is only the character identity, not the content theme. Do not add or write NightSailing, 夜航, 夜航船, boats, sails, sea waves, harbor, dock, lighthouse, moon, stars, navigation charts, anchors, portholes, or nautical scenery unless the source article explicitly asks for them. The visual metaphor must come from the article content only.

Theme:
{正文配图主题}

Structure type:
{结构类型：Workflow / 系统局部 / 前后对比 / 角色状态 / 概念隐喻 / 方法分层 / 地图路线 / 小漫画分镜}

Core idea:
{这张图要表达的核心意思}

Composition:
{具体画面：夜航猫头鹰在哪里、正在做什么、主要物件是什么、信息如何流动}

Suggested elements:
{元素1} / {元素2} / {元素3} / {元素4}

Chinese handwritten labels:
{标注词1} / {标注词2} / {标注词3} / {标注词4} / {可选标注词5}

Color use:
Black for main line art, outlines, handwritten text, and sunglasses. Owl colors: warm orange face/ear tufts, muted teal-blue feathers, deep blue robe, white coffee mug. Orange for main flow/path/arrows. Red only for key warnings/problems/results. Blue only for secondary notes or feedback/system state. Keep colors restrained.

Constraints:
One image explains only one core structure. Keep the main subject around 40%-60% of the canvas. Preserve at least 35% blank white space. Use at most 5-8 short handwritten Chinese labels. Do not write a title in the top-left corner. Do not write the structure type on the image. Do not make it a formal diagram, course slide, or dense explainer. Do not make the owl black or turn it into a black silhouette character. Do not make it cute, glossy, 3D, realistic, or heavily feathered. Do not copy prior examples; invent a fresh visual metaphor for this specific article. It should be clear but not instructional, interesting but not childish, strange but clean.
```

## 简化角色提示

只在用户明确要求“更简化 / 更符号化”时使用：

```text
Simplify only the 夜航猫头鹰 character. Keep its colors and identity, but reduce feather marks, robe folds, sleeve details, foot details, and decorative lines. Keep the warm orange face disk, two orange ear tufts, black sunglasses, blue robe, and white mug. Do not remove the owl identity and do not turn it into a black silhouette.
```

## 去除误入夜航概念提示

当生成结果把夜航概念带入内容时使用：

```text
Edit or regenerate the illustration while preserving the article concept and sparse hand-drawn layout. Remove all NightSailing/夜航/夜航船 text and all boats, sea waves, harbor, dock, lighthouse, moon, stars, anchors, portholes, navigation charts, and nautical scenery that were not explicitly part of the source article. Keep only the colored owl operator as the recurring character. Replace removed elements with plain white background or article-derived low-tech objects.
```
