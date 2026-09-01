# Moneta

「Contract · to · Cash」业务中台的**交互原型**与**品牌资产**仓库。
覆盖范围：客户引入 → 合同管理 → 计提 → 对账 → 开票 → 应收。

## 在线预览

- 索引页：https://jiajia11272042.github.io/moneta/
- 付款合同 + 权限改造（第二期）：https://jiajia11272042.github.io/moneta/payment-contract/

## 目录约定（后续 Moneta 相关内容统一放这里）

```
/index.html            原型索引页
/payment-contract/     付款合同 + 权限改造（第二期）原型
/brand/                品牌资产（logo / favicon / 横版字标）
```

新增模块时在根目录建子文件夹（如 `/accrual/`、`/invoice/`），并在 `index.html` 增加入口。

## 品牌资产

主标 = 契约方牌 + 衬线 M + 文书线 + 用印金点；主色 藏青 `#1e2a3a` · 暗金 `#C9A24B` · 象牙白 `#F3EEE3`。

前端接入 favicon：

```html
<link rel="icon" href="/favicon.ico" sizes="any">
<link rel="icon" type="image/svg+xml" href="/moneta-icon-simple.svg">
```

各文件用途见 `brand/README.md`。

## 说明

- 本仓库仅含**交互原型**（数据为 mock）与品牌资产，**不含需求文档**；PRD 维护在内部飞书。
- 原型用于评审沟通，交互与字段可能先于开发实现。
