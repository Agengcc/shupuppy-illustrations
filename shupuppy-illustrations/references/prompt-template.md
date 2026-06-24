# 生图提示词模板

每张图单独生成。根据正文内容替换变量，不要把多张图拼在一起。

```text
Generate one standalone 16:9 horizontal Chinese article illustration.

Visual DNA:
Pure white background. Healing colored-pencil / waxy crayon texture with visible grain. Dark-blue hand-drawn outlines. Small blue/yellow/red accent color blocks. Loose storybook feeling, but used for article concept illustration. Sparse handwritten Chinese annotations. Clean, warm, clever, and slightly mischievous. No gradients, no glossy shadows, no complex background, no photorealistic pet portrait, no commercial pet poster, no PPT infographic look, no formal flowchart, no cute sticker sheet.

Recurring IP character required:
薯条, a simple white picture-book dog character, not a realistic Bichon portrait. Round soft white head, large floppy ears, deliberately large round black nose as the main memory point, small black dot eyes, tiny paws, gentle calm expression, and a small colored bib/bandana. 薯条 feels relaxed, sociable, easygoing, and slightly mischievous. It must perform the core conceptual action in the illustration, not sit as a decorative cute pet. Keep the character visually consistent across images: white round head, big floppy ears, large black nose, small black dot eyes, small paws, and colored bib. Do not beautify the face by shrinking the nose or enlarging the eyes; the big nose and small eyes are the recognizable IP anchor.

Theme:
{正文配图主题}

Structure type:
{结构类型：叼走重点 / 暗中观察 / 整理资料 / 筛选信息 / 连接线索 / 修补流程 / 角色状态}

Core idea:
{这张图要表达的核心意思}

Composition:
{具体画面：薯条在哪里、正在做什么、主要物件是什么、信息如何流动}

Suggested elements:
{元素1} / {元素2} / {元素3} / {元素4}

Chinese handwritten labels:
{标注词1} / {标注词2} / {标注词3} / {标注词4}

Color use:
Dark blue for hand-drawn outlines, structure lines, and arrows. White for 薯条 and background. Light gray or warm cream for subtle fur texture. Yellow for main path, clue, or soft highlight. Red only for small warnings, problem dots, or tiny bib accents. Black only for 薯条's nose and eyes.

Constraints:
One image explains only one core structure. Keep the main subject around 40%-60% of the canvas. Preserve lots of blank white space. Use at most 3-6 short handwritten Chinese labels. Do not write a title in the top-left corner. Do not write the structure type on the image. Do not make it a pet portrait, cute avatar, formal diagram, course slide, or dense explainer. Do not make 薯条 decorative; 薯条 must be doing the conceptual work. Do not shrink the nose, enlarge the eyes, remove the floppy ears, or remove the colored bib. It should feel like a warm colored-pencil article illustration, not a pet photo or PPT.
```

## 图像编辑提示

去掉左上角标题：

```text
Edit the provided image. Remove only the handwritten title "{要删除的文字}" and its underline from the top-left corner. Fill that area with the same clean white background, matching the surrounding blank paper. Preserve everything else exactly: 薯条, labels, paths, line style, composition, aspect ratio, and image quality. Do not add any new text or objects.
```

增强薯条参与感：

```text
Regenerate this illustration with the same core meaning and simple layout, but make 薯条 more central to the conceptual action. 薯条 should be doing the work that explains the idea, such as biting, observing, sorting, filtering, connecting, or repairing. Keep the colored-pencil texture, dark-blue outlines, white background, and blue/yellow/red accents. Do not make 薯条 a decorative cute pet.
```

修正 IP 漂移：

```text
Regenerate this illustration while preserving the same idea and composition. Make 薯条 match the approved IP more closely: white round head, big floppy ears, deliberately large black round nose, small black dot eyes, tiny paws, and a small colored bib. Do not make it a realistic Bichon, generic puppy, pet portrait, or cute sticker.
```

