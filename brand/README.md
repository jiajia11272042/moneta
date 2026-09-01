# Moneta 品牌资产交接说明（给前端）

主标：契约方牌 + 衬线 M + 文书线 + 用印金点
配色：藏青 #1e2a3a · 暗金 #C9A24B · 象牙白 #F3EEE3

## 浏览器页签（favicon）
- `favicon.ico`：多分辨率 16/32/48/64，标准 MS Windows icon（RGBA）
- `favicon-16/32/48/64.png`：备用 PNG
- `moneta-icon-simple.svg`：矢量简化版（现代浏览器优先）

接入（把文件放到工程 public/ 或 static/ 根目录）：
```html
<link rel="icon" href="/favicon.ico" sizes="any">
<link rel="icon" type="image/svg+xml" href="/moneta-icon-simple.svg">
```
> 说明：**所有尺寸均保留文书线（横条）**。为保证小尺寸可辨识，按尺寸做了优化：
> - 16px：去掉内框降噪、M 放大、横线加粗（像素级验证可见 2 条横条）
> - 32px：内框略粗、横线加粗
> - 48/64px：使用标准主标（细内框 + 细横线）

## 平台内 Logo
- `moneta-icon-full.svg`（主标，带文书线，推荐 UI 内使用）/ `moneta-icon-full-512.png`
- `moneta-icon-mono.svg`（单色版）
- 横版字标：`moneta-lockup-dark.svg`（深色底/侧边栏）、`moneta-lockup-light.svg`（浅色底）、`moneta-lockup-mono.svg`（单色）+ 同名 PNG

## 备注
- SVG 中 M 使用 Georgia/Times 衬线字体族；若需完全避免字体依赖，可让设计把 M 转为路径（outline）后再交付。
- 生成脚本：build_brand.py（可调整尺寸/配色后重新导出）
