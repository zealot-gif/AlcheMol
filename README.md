# 🧪 AlcheMol — Interactive 2D/3D Chemical Structure Editor & Viewer

[繁體中文](#繁體中文) | [English](#english)

---

## 繁體中文

**AlcheMol** 是一款純前端、無需後端伺服器的互動式化學分子繪圖與 3D 結構視覺化網頁應用程式。專為有機化學學習、反應機構推演與立體構象觀察設計，支援即時 2D 鍵線式繪製、自動八隅體與隱含氫原子計算、結構異構物辨識，以及 3D 分子構象轉換與單鍵二面角（Torsion Angle）旋轉。

### ✨ 核心功能

* **直覺式 2D 化學繪圖畫布**
  * **完整鍵結與原子工具：** 支援單鍵、雙鍵、三鍵切換，常見有機元素快速選單，以及完整元素週期表。
  * **智慧有機化學價數引擎：** 依據八隅體法則與實際鍵結數，自動即時計算並顯示隱含氫原子（如 `-CH₃`、`-NH₂`）與形式電荷（支援四級銨鹽 `R₄N⁺`、葉立德 Ylide 與超價雜原子），並可一鍵切換「顯示 / 隱藏 2D 氫原子 (`H`)」。
  * **反應機構專用工具：** 內建 VSEPR 物理排斥自動定位的孤電子對（`：:`）與可自由調整弧度與去回方向的電子轉移彎箭頭（`↷`）。
  * **豐富環狀與官能基模板：** 支援拖曳動態調整 3～18 員多邊形環，內建芳香環與生醫環庫（苯、萘、蒽、菲、嘌呤、嘧啶、吡啶、哌啶）及常見取代基（`-CH₃`、`-OH`、`-COOH`、`-NO₂`、`-CN`、`-Ph` 等）。
  * **結構優化與構象轉換：** 支援一鍵結構自動重整拉正（`✨`）與六員環椅型構象 / 環翻轉（Chair Flip `🪑`）。
* **多維度搜尋與異構物辨識**
  * 支援**中文俗名、英文 IUPAC 名稱、SMILES** 與 **分子式（如 `C4H10`、`C2H6O`、`C6H12O6`）** 檢索。
  * 輸入含多種結構的分子式時，自動彈出**結構異構物選擇視窗**並附帶 2D 骨架縮圖預覽。
* **即時 3D 分子視覺化與構象分析**
  * 支援一鍵將 2D 畫布（包含帶電荷物種與多分子系統）轉換為 3D 立體構象。
  * 提供**球棍模型 (Ball & Stick)**、**空間填充 (Space-filling)** 與 **線框模型 (Wireframe)** 三種渲染模式。
  * **單鍵二面角旋轉器：** 自動偵測可旋轉單鍵，透過滑桿即時觀察交錯式（Staggered）與重疊式（Eclipsed）構象變化。
  * 支援匯出標準 `.sdf`（MDL SDfile）3D 分子結構檔案。
* **跨裝置響應式體驗**
  * 桌面版支援可自由拖曳寬度比例的 2D / 3D 雙分割視窗；手機與平板版提供緊湊工具列、雙指縮放旋轉手勢與單鍵視圖切換。

### 🕹 操作說明

| 操作 / 工具 | 功能說明 |
| :--- | :--- |
| **✋ 移動模式** | 拖曳單一分子可調整獨立位置；拖曳空白處可平移整個畫布。 |
| **滑鼠右鍵拖曳 / 雙指手勢** | 旋轉整個 2D 畫布視角並同步縮放比例。 |
| **滑鼠滾輪** | 放大或縮小 2D 繪圖畫布（30% ～ 300%）。 |
| **⬡ 多邊形環工具** | 單擊放置六員環；按住並向外拖曳可動態調整 3 至 18 員環與角度。 |
| **🪑 椅型構象按鈕** | 將畫布中的封閉六員環轉換為椅型構象（Chair），再次點擊可執行環翻轉（Ring Flip）。 |
| **⚡ 轉 3D 按鈕** | 將目前 2D 畫布中的所有分子同步演算並渲染至右側 3D 視窗。 |
| **💾 保存按鈕** | 將目前的 3D 分子結構匯出下載為 `molecule_3d.sdf`。 |

### 🚀 部署與執行

本專案為純靜態網頁（HTML / CSS / Vanilla JavaScript），無需建置步驟（Zero-Build）：
1. 下載或 Clone 本儲存庫。
2. 直接使用瀏覽器開啟 `index.html`，或透過任何靜態網頁伺服器（如 VS Code Live Server、GitHub Pages）託管即可使用。

---

## English

**AlcheMol** is a zero-backend, browser-based interactive 2D chemical structure editor and 3D molecular viewer. Built for organic chemistry education, reaction mechanism illustration, and stereochemical conformation analysis, it combines real-time 2D skeletal drawing, automated valence/implicit hydrogen calculation, constitutional isomer recognition, and interactive 3D conformer generation with rotatable torsion angles.

### ✨ Key Features

* **Intuitive 2D Chemical Sketcher**
  * **Bonds & Elements:** Draw single, double, and triple bonds; quick-access common organic elements plus a full interactive Periodic Table.
  * **Smart Organic Valence Engine:** Automatically calculates implicit hydrogens and formal charges based on octet rules and actual bond orders (supporting quaternary ammonium `R₄N⁺`, ylides, and hypervalent heteroatoms). Includes a one-click toggle (`H`) to expand or collapse 2D hydrogens.
  * **Reaction Mechanism Tools:** Place VSEPR-positioned lone pairs (`：:`) and curved electron-pushing arrows (`↷`) with adjustable curvature and direction flipping.
  * **Rings & Substituent Templates:** Click to place cyclohexane or drag dynamically for 3–18 membered rings. Includes built-in aromatic/biochemical ring templates (benzene, naphthalene, anthracene, phenanthrene, purine, pyrimidine, pyridine, piperidine) and common functional groups (`-CH₃`, `-OH`, `-COOH`, `-NO₂`, `-CN`, `-Ph`, etc.).
  * **2D Clean-Up & Chair Conformation:** Auto-beautify bond angles (`✨`) and convert 6-membered rings into chair conformations with interactive ring flipping (`🪑`).
* **Smart Search & Isomer Picker**
  * Search compounds by **English/Chinese names, SMILES strings**, or **molecular formulas** (e.g., `C4H10`, `C2H6O`, `C6H12O6`).
  * Automatically detects constitutional/stereoisomers for a given formula and presents a visual selection modal with 2D skeletal thumbnails.
* **Interactive 3D Molecular Viewer**
  * Convert 2D drawings—including charged species and multi-component systems—into 3D conformers on the fly.
  * Switch between **Ball & Stick**, **Space-filling**, and **Wireframe** rendering styles.
  * **Single-Bond Torsion Rotator:** Automatically identifies rotatable single bonds and lets you scrub dihedral angles (`0°–360°`) to inspect staggered vs. eclipsed conformations.
  * Export 3D coordinates as standard `.sdf` (MDL SDfile) files.
* **Responsive Desktop & Mobile Design**
  * Desktop features a draggable split-pane layout; mobile devices feature compact toolbars, two-finger pinch-to-zoom/rotate gestures, and seamless 2D/3D view toggling.

### 🕹 Controls & Shortcuts

| Action / Tool | Description |
| :--- | :--- |
| **✋ Move Tool** | Drag an individual molecule to reposition it, or drag empty canvas space to pan. |
| **Right-Click Drag / 2-Finger Gesture** | Rotate and zoom the 2D canvas simultaneously. |
| **Mouse Wheel** | Zoom in/out of the 2D canvas (`30% – 300%`). |
| **⬡ Polygon Ring Tool** | Click to place a 6-membered ring, or click-and-drag to dynamically adjust ring size (`3–18`) and orientation. |
| **🪑 Chair Conformation** | Converts a closed 6-membered ring into a chair conformation; click again to perform a chair flip. |
| **⚡ Convert to 3D (`轉 3D`)** | Computes and renders the 3D conformer(s) of the current 2D canvas. |
| **💾 Save (`保存`)** | Exports the active 3D structure as `molecule_3d.sdf`. |

### 🚀 Getting Started

This project uses pure HTML5, CSS3, and Vanilla JavaScript with zero build dependencies:
1. Clone or download this repository.
2. Open `index.html` directly in any modern web browser, or deploy via GitHub Pages.

---

## 📜 Open Source Acknowledgments & Licenses / 開源授權與資料致謝

This project is powered by the following open-source libraries and public scientific databases:

* **[3Dmol.js](https://3dmol.csb.pitt.edu/)** — WebGL-accelerated 3D molecular visualization library. Licensed under the **BSD 3-Clause License**.
* **[OpenChemLib JS](https://github.com/cheminfo/openchemlib-js)** — Cheminformatics engine used for SMILES/Molfile parsing, 2D coordinate generation, molecular formula calculation, and 3D conformer generation. Licensed under the **BSD 3-Clause License**.
* **[PubChem (NCBI / NIH)](https://pubchem.ncbi.nlm.nih.gov/)** — Public chemical structure and property data retrieved via the PubChem PUG REST API.
* **Disclaimer / 免責聲明：** AlcheMol is an independent educational and research visualization tool and is not affiliated with or endorsed by MolView.

## 📄 License

The original source code of **AlcheMol** is licensed under the **MIT License**.
