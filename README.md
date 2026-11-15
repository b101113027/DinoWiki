# 🦕 恐龍百科資料庫 (DinoWiki)

歡迎來到 **DinoWiki**。本資料庫是一個以現代脊椎動物古生物學（Vertebrate Paleontology）科學共識為核心的結構化知識庫，致力於提供科學嚴謹、分類完整且語言生動的中生代恐龍百科。

---

## 🧭 資料庫結構導覽

```text
dinowiki/
├── AGENTS.md                         # 🤖 AI Agent 協作指南、科學規則與強制校驗清單
├── README.md                         # 📖 專案索引與入口文件
├── templates/                        # 📝 標準化 Markdown 模板
│   ├── species-template.md           # 物種檔案卡模板 (Species Card)
│   └── topic-template.md             # 專題條目模板 (Topic Overview)
├── glossary/                         # 📚 專有名詞標準對照字典
│   └── terminology.md                # 地質年代、分類階元與解剖構造中英拉丁對照
├── wiki/                             # 🦖 百科條目核心庫
│   ├── 01-origins-and-evolution/     # 起源、三疊紀輻射與生態位演替
│   ├── 02-taxonomy/                  # 恐龍分類學（骨盆結構、蜥臀目 vs 鳥臀目）
│   ├── 03-carnivores/                # 肉食性恐龍（暴龍、伶盜龍）
│   ├── 04-herbivores/                # 植食性恐龍（三角龍、劍龍、巨型蜥腳類）
│   ├── 05-behavior-and-reproduction/ # 生活習性、繁殖孵化與親代撫育
│   └── 06-extinction/                # 白堊紀—古近紀滅絕事件 (K-Pg)
└── assets/                           # 🖼️ 圖表與解剖示意資源庫
```

---

## 📚 精選核心條目索引

| 類別 / 主題 | 條目名稱 | 英文 / 學名 | 關鍵探討主題 |
| :--- | :--- | :--- | :--- |
| **01. 起源與演化** | [恐龍的起源與演化](wiki/01-origins-and-evolution/index.md) | Origin & Evolution | 主龍類演化、雙足直立、三疊紀至白堊紀生態位更替 |
| **02. 恐龍分類學** | [恐龍分類學與骨盆結構](wiki/02-taxonomy/index.md) | Taxonomy & Pelvic Morphology | 腸骨/坐骨/恥骨、蜥臀目、鳥臀目、鳥類起源悖論 |
| **03. 肉食性恐龍** | [君王暴龍](wiki/03-carnivores/tyrannosaurus-rex.md) | *Tyrannosaurus rex* | 8-9 噸體重修正、碎骨咬合力、立體視覺、前肢功能 |
| **03. 肉食性恐龍** | [蒙古伶盜龍](wiki/03-carnivores/velociraptor-mongoliensis.md) | *Velociraptor mongoliensis* | 火雞體型、羽莖瘤羽毛鐵證、第二趾鐮刀爪、群獵迷思 |
| **04. 植食性恐龍** | [前後三角龍](wiki/04-herbivores/triceratops-prorsus.md) | *Triceratops prorsus* | 實心頭盾、剪切型齒電池、同種角鬥穿刺傷 |
| **04. 植食性恐龍** | [窄臉劍龍](wiki/04-herbivores/stegosaurus-stenops.md) | *Stegosaurus stenops* | 交錯骨板、**尾刺 (Thagomizer)** 嚴格辨析、非尾槌 |
| **04. 植食性恐龍** | [巨型蜥腳下目概論](wiki/04-herbivores/sauropoda-overview.md) | Sauropoda Overview | 蜥臀巨獸、骨骼氣腔化、長頸採食、胃石消化 |
| **05. 生活與繁殖** | [恐龍生活、繁殖與親代撫育](wiki/05-behavior-and-reproduction/index.md) | Paleoethology & Reproduction | 竊蛋龍抱卵平反、慈母龍集群築巢育幼、中溫性 |
| **06. 恐龍滅絕** | [白堊紀—古近紀滅絕事件](wiki/06-extinction/k-pg-event.md) | K-Pg Extinction Event | 希克蘇魯伯撞擊、撞擊冬天、德干火山、鳥類倖存 |

---

## 🛡️ 資料品質與 Agent 撰寫準則

所有條目均嚴格遵從 [`AGENTS.md`](AGENTS.md) 的規範：
1. **中英雙語標註**：正體中文為主，所有物種首次出現均標註斜體學名（如 *Tyrannosaurus rex*）。
2. **科學糾錯紅線**：
   * 劍龍尾部防禦構造為 **「尾刺 (Thagomizer)」**，嚴禁稱為「尾槌 (Tail club)」。
   * 暴龍成體體重依據現代 3D 容積重建為 **8 至 9.5 公噸**，拒絕過時低估數據。
   * 伶盜龍具備羽莖瘤與覆蓋羽毛，其體型接近火雞，非高大人形尺寸。
   * 現代鳥類為現生「鳥類恐龍 (Avian Dinosaurs)」，滅絕者為「非鳥恐龍 (Non-avian Dinosaurs)」。
