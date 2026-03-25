# 數位影像處理 / Digital Image Processing

| 項目 | 資訊 |
|------|------|
| **姓名** | 馬盛中 |
| **學號** | 4B1YZ001 |
| **學校** | 南台科技大學 |
| **課程** | 數位影像處理 |

---

## 📁 專案結構

```
digital_image_processing/
├── 0001_Image_Display.ipynb          ☁️  Colab 版本
├── 0001_Image_Display_Jupyter.ipynb  🖥️  Jupyter 本地版本
├── database/                          影像資料夾
│   ├── Lenna.jpg
│   ├── Lenna_2.bmp
│   └── Baboon.bmp
└── README.md
```

---

## 📓 Notebook 版本說明

本專案提供兩個版本的 notebook，功能相同但執行環境不同：

### ☁️ `0001_Image_Display.ipynb` — Google Colab 版本

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mendresvon/digital_image_processing/blob/main/0001_Image_Display.ipynb)

- 需掛載 **Google Drive** 並將影像放置於 `/MyDrive/Colab/Colab_Database/`
- 使用 `cv2_imshow(img)` 顯示影像（Colab 專用）
- 不支援 `cv2.imshow()` / `cv2.waitKey()` / `cv2.destroyAllWindows()`
- 部分視窗控制功能已標記跳過

### 🖥️ `0001_Image_Display_Jupyter.ipynb` — 本地 Jupyter 版本

- 使用本地相對路徑 `./database/`，**無需** Google Drive
- 使用 `matplotlib` inline 顯示影像（推薦）
- **完整支援** `cv2.imshow()` / `cv2.waitKey()` / `cv2.destroyAllWindows()`
- 包含 Colab 版本中跳過的所有範例（視窗控制、namedWindow 等）

### 主要差異對照表

| 功能 | Colab 版本 | Jupyter 版本 |
|------|:---------:|:----------:|
| 執行環境 | Google Colab | 本地 Jupyter |
| 影像路徑 | Google Drive | `./database/` |
| 顯示方式 | `cv2_imshow()` | `plt.imshow()` |
| `cv2.imshow()` 視窗 | ❌ 不支援 | ✅ 支援 |
| `cv2.waitKey()` | ❌ 不支援 | ✅ 支援 |
| `cv2.namedWindow()` | ❌ 不支援 | ✅ 支援 |
| 需要掛載 Drive | ✅ 是 | ❌ 否 |

---

## 🚀 使用方式

### Colab 版本
1. 點擊上方 "Open in Colab" 徽章
2. 執行第一格，掛載 Google Drive
3. 將 `database/` 資料夾上傳至 `/MyDrive/Colab/Colab_Database/`
4. 依序執行各格

### Jupyter 本地版本
1. Clone 此 repo
2. 確認 `database/` 資料夾存在且包含影像檔案
3. 啟動 Jupyter Notebook 或 JupyterLab
4. 開啟 `0001_Image_Display_Jupyter.ipynb`
5. 依序執行各格
