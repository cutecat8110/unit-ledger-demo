# 度冊計費｜表計與帳務管理

`Nuxt 4` · `Vue 3` · `TypeScript` · `Nuxt UI` · `IndexedDB`

批次抄表、總分表核對、費率試算與帳單管理。

**[開啟 Demo](https://cutecat8110.github.io/unit-ledger-demo/)**

![批次抄表與總分表用量核對](docs/images/readings.png)

| 入口 | 代表操作 |
| --- | --- |
| [表計管理](https://cutecat8110.github.io/unit-ledger-demo/#/meters) | 總分表關聯、查詢、編修與匯出 |
| [批次抄表](https://cutecat8110.github.io/unit-ledger-demo/#/readings) | CSV 預覽、整批驗證與用量核對 |
| [費率試算](https://cutecat8110.github.io/unit-ledger-demo/#/calculator) | 階梯費率、基本費、稅額及出帳快照 |
| [帳單查詢](https://cutecat8110.github.io/unit-ledger-demo/#/bills) | 明細、確認／撤回及 CSV 匯出 |

**試用：** 點鑰匙帶入帳密 → 補登 2026 年 9 月讀數 → 選群組核對 → 試算出帳 → 查看明細。

<details>
<summary>費率試算與帳單明細</summary>

![階梯費率與試算結果](docs/images/calculator.png)
![帳單費用明細](docs/images/bills.png)

</details>

<details>
<summary>角色與使用說明</summary>

帳務管理可編修表計與出帳；抄表作業可登錄、試算與查看帳單。

資料與費率供展示，權限由前端模擬，修改保存在目前瀏覽器。沒有跨裝置同步、付款或正式帳務串接；「重設資料」恢復初始內容。

CSV 使用頁面提供的 UTF-8 範本，驗證後帶入表格，另按「儲存讀數」。用量核對採已存讀數；缺表或區間不同不計差額，也不自動分攤。出帳會鎖定相關讀數，待確認帳單可撤回，已確認帳單不可撤回。

</details>
