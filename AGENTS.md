# AGENTS.md - 恐龍百科資料庫 (DinoWiki) 協作與維護規範

本文件為 **DinoWiki** 的代理人（Agents）與維護者協作協議。所有參與本資料庫條目生成、事實校對、分類修訂與跨鏈接更新的 Agent，均須嚴格遵守以下準則。

---

## 1. 專案宗旨與核心定位 (Project Mission)

* **核心目標**：建構科學嚴謹、資料架構完整、符合現代古生物學（Vertebrate Paleontology）共識的恐龍與中生代百科庫。
* **語言政策**：以**正體中文為主**，所有專有名詞、生物學名、解剖學構造、地質年代與分類階元於各章節初次出現時，**必須並列標準英文或拉丁學名**（例：君王暴龍 *Tyrannosaurus rex*、白堊紀—古近紀滅絕事件 (K-Pg extinction event)）。
* **受眾定位**：兼顧學術正確性與科普可讀性，破除常見通俗文化謬誤（如侏羅紀公園效應、傳統冷血蜥蜴刻板印象）。

---

## 2. 目錄架構與職責邊界 (Repository Structure)

```text
dinowiki/
├── AGENTS.md                         # Agent 協作指南、科學規則與驗證清單
├── README.md                         # 專案入口導引與資料庫索引
├── templates/                        # 條目規範模板
│   ├── species-template.md           # 物種檔案卡模板
│   └── topic-template.md             # 專題與概論文章模板
├── glossary/                         # 詞彙索引與對照
│   └── terminology.md                # 核心中英拉丁專有名詞對照表
├── wiki/                             # 百科核心內容
│   ├── 01-origins-and-evolution/     # 起源、三疊紀輻射與生態位演替
│   ├── 02-taxonomy/                  # 恐龍分類學（蜥臀目 vs 鳥臀目）
│   ├── 03-carnivores/                # 肉食性恐龍、頂級掠食者與獸腳類
│   ├── 04-herbivores/                # 植食性恐龍、齒系與裝甲演化
│   ├── 05-behavior-and-reproduction/ # 生理代謝、親代撫育與社會行為
│   └── 06-extinction/                # K-Pg 滅絕事件、隕石撞擊與鳥類倖存
└── assets/                           # 圖表、骨骼圖解與地層剖面圖資
```

---

## 3. 古生物學事實與校對紅線 (Fact-Checking & Anti-Misconception Rules)

所有 Agent 在撰寫或審查條目時，必須執行下列強制事實校驗（違反即判定為致命錯誤）：

### 規則 3.1：物種命名與書寫格式
1. **二名法斜體規則**：屬名 (Genus) 與種加詞 (Specific epithet) **必須使用斜體**。屬名首字母大寫，種加詞全小寫。
   * 正確：君王暴龍 *Tyrannosaurus rex*（簡寫為 *T. rex*）、蒙古伶盜龍 *Velociraptor mongoliensis*。
   * 錯誤：Tyrannosaurus Rex、*T-Rex*、三角龍 triceratops。
2. **更高階元格式**：科 (Family)、目 (Order)、演化支 (Clade) 等階元使用正體首字母大寫（如 Theropoda、Ornithischia）。

### 規則 3.2：嚴禁名詞混淆與解剖構造錯誤
* ❌ **劍龍的防禦構造**：嚴禁將劍龍尾部的 4 根尖刺稱為「尾槌 (Tail club)」。劍龍尾部構造的正式名稱為 **「尾刺 (Thagomizer)」**。
* ❌ **尾槌的歸屬**：**「尾槌 (Tail club)」** 為 **甲龍亞目（Ankylosauria，特別是甲龍科 Ankylosauridae）** 的骨質末端錘狀特徵。
* ❌ **恐龍咀嚼機制**：嚴禁寫「恐龍下頜能像牛羊般靈活左右研磨」。恐龍缺乏哺乳類的下頜橫向研磨關節；鴨嘴龍類與角龍類是藉由 **顱骨可動性研磨 (Cranial kinesis / Pleurokinesis)** 或 **前後向滑動研磨 (Propalinal chewing)** 配合齒電池進行剪切與磨碎。

### 規則 3.3：體型與體重數據更新
* ❌ 暴龍成體體重**嚴禁使用過時的 5~6 公噸**。基於現代 3D 骨骼激光掃描與容積重建（如標本 "Sue" 與 "Scotty"），成體暴龍的科學推估體重為 **8 至 9.5 公噸 (Metric tons)**。

### 規則 3.4：行為與羽毛的科學邊界
* ⚠️ **伶盜龍 (Velociraptor) 的生態還原**：
  * **體型**：真實體型僅如火雞或土狼大小（長約 2 公尺、臀高約 0.5 公尺、體重約 15~20 公斤），非電影中高大的人形尺寸。
  * **羽毛**：前肢尺骨具清晰的「羽莖瘤 (Quill knobs)」，證實其覆蓋完整的正羽與羽翼。
  * **圍獵行為**：現代古生物學界對馳龍類具備「高度溝通與組織化群獵」持高度懷疑，應客觀陳述為「獨居伏擊或似現代巨蜥般的群聚爭食（Opportunistic mobbing）」。
* ⚠️ **竊蛋龍 (*Oviraptor*) 的平反**：
  * 必須強調 1923 年發現時被誤認為「偷原角龍蛋的賊」，1990 年代蒙古戈壁的新化石證實其是在以鳥類姿態**趴伏在自身蛋巢上孵卵護幼**。

### 規則 3.5：分類學與滅絕命名標準
* **鳥類本質**：現代鳥類在系統發育學上屬於 **「鳥類恐龍 (Avian dinosaurs)」**。因此，白堊紀末期滅絕的是 **「非鳥恐龍 (Non-avian dinosaurs)」**，不能籠統稱「恐龍已完全滅絕」。
* **骨盆命名陷阱**：明確強調「鳥類演化自蜥臀目（獸腳類），而非鳥臀目」。
* **滅絕事件代號**：必須使用國際地層委員會 (ICS) 標準名稱 **「白堊紀—古近紀滅絕事件 (K-Pg extinction event)」**；若提及舊稱「K-T 滅絕」，須註明第三紀 (Tertiary) 已被古近紀 (Paleogene) 與新近紀 (Neogene) 取代。
* **滅絕成因多元性**：除希克蘇魯伯小行星撞擊 (Chicxulub impact) 為直接誘因外，應提及印度德干暗色岩 (Deccan Traps) 大規模火山作用對全球生態系造成的背景壓力。

---

## 4. 條目撰寫標準 (Formatting & Style)

1. **Frontmatter 元資料**：所有物種與專題條目頂部必須包含 YAML 區塊：
   ```yaml
   ---
   id: tyrannosaurus-rex
   title: 君王暴龍
   scientific_name: Tyrannosaurus rex
   clade: Dinosauria > Saurischia > Theropoda > Tyrannosauridae
   period: 白堊紀晚期 (Late Cretaceous, ~68–66 Ma)
   diet: 肉食性 (Carnivore)
   estimated_mass: 8,000–9,500 kg
   status: extinct
   last_reviewed: 2026-11-15
   ---
   ```
2. **段落必備模組**：
   * **分類階元與歷史** (Taxonomy & History)
   * **形態特徵與解剖學** (Morphology & Anatomy)
   * **古生態學與食性** (Paleoecology & Diet)
   * **化石發現與關鍵標本** (Fossil Record & Key Specimens)
   * **科學迷思與破除** (Myths vs Scientific Evidence)
   * **參考文獻與館藏來源** (References & Museum Sources)

---

## 5. Agent 角色分工矩陣 (Agent Personas)

| 角色名稱 (Persona) | 主要職責 | 關鍵檢查項目 |
| :--- | :--- | :--- |
| **Wiki-Curator (典藏架構官)** | 維護目錄樹、交叉雙向鏈接、模板一致性 | 檢查 YAML 標籤、檢查 Wiki 內部鏈接無死鏈 |
| **Paleo-Fact-Checker (古生物校對員)** | 檢驗體重、地層年代、食性特化與學術論文數據 | 檢查第 3 節列出的所有紅線與事實錯誤 |
| **Taxonomy-Librarian (分類學管理員)** | 維護系統發生樹 (Phylogenetic tree) 與學名有效性 | 檢查二名法斜體、種屬關聯、蜥臀目/鳥臀目歸屬 |

---

## 6. 新條目生成與修訂檢查清單 (Agent Verification Checklist)

在標記任何任務完成前，Agent 必須逐項核對：
- [ ] 屬名與種名是否完整斜體（如 *Tyrannosaurus rex*）？
- [ ] 中文名稱是否隨附標準英文或拉丁專有名詞？
- [ ] 是否已校驗防禦結構名稱（無「劍龍尾槌」，正確使用「尾刺 Thagomizer」與「尾槌 Tail club」）？
- [ ] 暴龍體重與伶盜龍羽毛／行為是否符合現代古生物學共識？
- [ ] 植食性恐龍是否涵蓋蜥腳下目 (Sauropoda)？
- [ ] 滅絕事件是否標記為 K-Pg，並指出鳥類即現生恐龍？
- [ ] 條目是否引用了權威來源（如科博館、香港科學館、自然史博物館或同行評審文獻）？
