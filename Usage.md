# ISIP.HS Slidev 主題使用指南

## 簡介

ISIP.HS Slidev 主題是一個專為先進資通安全人才培育計劃高中職資安教學資源與推廣中心（ISIP.HS）設計的 [Slidev](https://github.com/slidevjs/slidev) 簡報主題。該主題提供了一系列精美的版面配置和樣式，幫助您快速創建符合 ISIP.HS 設計標準的專業簡報。

> [!NOTE]
> 本主題所使用之圖片，若有違反版權，請至 issue 聲明。作者將會收到 issue 後盡快下架該圖片。

## 安裝

要使用此主題，請在您的 `slides.md` 檔案的 frontmatter 中新增以下內容：

```yaml
---
theme: @cxphoenix/slidev-theme-isip.hs
---
```

如果您是第一次使用此主題，Slidev 將提示您自動安裝。

或者，您可以透過 npm/yarn/pnpm 手動安裝：

```bash
# 使用 npm
npm install @cxphoenix/slidev-theme-isip.hs

# 使用 yarn
yarn add @cxphoenix/slidev-theme-isip.hs

# 使用 pnpm
pnpm add @cxphoenix/slidev-theme-isip.hs
```

## 主題特色

### 字型

本主題預設使用：
- 正文字型：Noto Sans TC
- 等寬字型：Fira Code

### 版面配置

本主題提供以下幾種版面配置：

#### 1. 封面版面 (cover)

這是預設版面，用於簡報的第一頁。它包含標題、副標題和 ISIP.HS 標誌。

範例用法：
```markdown
---
theme: @cxphoenix/slidev-theme-isip.hs
---

::title::
# 您的簡報標題

::subtitle::
## 您的簡報副標題
```

#### 2. 一般版面 (default)

用於大多數內容投影片。

範例用法：
```markdown
---

::title::
# 投影片標題

::default::
- 項目 1
- 項目 2
  - 子項目 A
  - 子項目 B
```

#### 3. 章節版面 (section)

用於分隔不同章節的投影片。

範例用法：
```markdown
---
layout: section
---

::title::
# 章節標題

::subtitle::
## 章節副標題
```

#### 4. 圖片版面 (image)

專為展示圖片設計的版面。

範例用法：
```markdown
---
layout: image
---

::title::
# 圖片標題

::default::
![描述](圖片路徑)
```

### 插槽

本主題使用以下命名插槽：

- `::title::` - 用於放置投影片標題
- `::subtitle::` - 用於放置投影片副標題
- `::default::` - 用於放置預設內容

## 樣式指南

### 標題

主題為不同等級的標題提供了特定樣式：

- `h1` - 用於主標題，尺寸為 3.3rem
- `h2` - 用於副標題，尺寸為 5xl
- `h3` - 用於小標題，尺寸為 4xl

### 列表

列表有專門的樣式設計：

- 一級列表項使用 "❖" 作為標記
- 二級列表項使用 "➢" 作為標記
- 三級列表項使用 "◼︎" 作為標記

範例：
```markdown
- 一級列表項
  - 二級列表項
    - 三級列表項
```

## 最佳實踐

1. **標題使用**：始終在 `::title::` 插槽中使用 `h1` 標籤作為投影片標題。
2. **內容分配**：將主要內容放置在 `::default::` 插槽中。
3. **圖片展示**：對於展示大圖片的投影片，使用 `image` 版面以獲得最佳顯示效果。
4. **章節劃分**：使用 `section` 版面來明確表示新章節的開始。

## 範例

完整的範例可以參考主題套件中的 `example.md` 檔案。

## 自訂

如果您需要自訂主題，可以覆蓋樣式或擴展版面配置。請參考 [Slidev 主題自訂指南](https://sli.dev/guide/write-theme.html) 獲取更多資訊。

## 問題排除

如果您在使用過程中遇到任何問題，請確保：

1. 您已經正確安裝了主題
2. 您的 frontmatter 中正確指定了主題
3. 您的 Slidev 版本支援該主題

如果問題仍然存在，請在 [GitHub Repository](https://github.com/CXPhoenix/slidev-theme-isip.hs) 提交 issue。 