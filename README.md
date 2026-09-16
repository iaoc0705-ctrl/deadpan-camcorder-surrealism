# Deadpan Camcorder Surrealism / 冷面DV超现实

一个用于生成“像被普通人偶然拍到”的超现实照片的 Codex Skill。它把乏味、可信的日常空间与一个清晰的物理悖论放在同一画面里，再用晚期 VHS / 早期 MiniDV 家用摄像机的质感，让荒诞事件看起来像真实记录。

## 最简用法

```text
使用 $deadpan-camcorder-surrealism 生成：场景 + 一个反常识事件。
```

例如：

```text
使用 $deadpan-camcorder-surrealism 生成：市政工人用一条巨型拉链修补开裂的马路。
```

当没有指定数量时，Skill 会先构思三个文字方案，选择最强的一个，再生成一张图片。也可以明确指定数量、画幅或仅要求提示词。

## 特点

- 普通地点里只出现一个容易理解的异常事件。
- 人物继续工作、排队或等待，不做夸张反应。
- 强调重量、接触、投影、磨损和环境反馈，让悖论具有物理可信度。
- 使用真实的消费级 MiniDV / VHS 摄像机语言，而不是现代照片叠加复古滤镜。
- 默认生成前进行概念筛选，避免为了数量堆叠低质量变体。
- 参考图只用于提炼视觉语言，不复刻人物、地点、动作或标志性画面。

## 示例

### 用拉链修马路

![用拉链修马路](examples/01-road-zipper.png)

### 自动洗车机清洗上班族

![自动洗车机清洗上班族](examples/02-human-car-wash.png)

### 医生给救护车做手术

![医生给救护车做手术](examples/03-ambulance-surgery.png)

### 牙医给汽车轮胎看牙

![牙医给汽车轮胎看牙](examples/04-dentist-tire.png)

## 安装

将本仓库克隆或解压到 Codex skills 目录，使结构如下：

```text
skills/
└── deadpan-camcorder-surrealism/
    ├── SKILL.md
    ├── agents/
    └── references/
```

随后在对话中使用 `$deadpan-camcorder-surrealism` 调用。图片生成依赖 Codex 内置 `image_gen`。

## 当前版本

`v0.1.0`：支持原创文生图、参考帧视觉语言提炼、概念筛选和单点修正。

## License

[MIT](LICENSE)
