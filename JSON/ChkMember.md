<div><h1>傳入 JSON</h1></div>

```json
{
  "group": "CA202.信豪牧區-彥伯小組",
  "Ename": "劉彥伯",
  "Phone": "0919963322"
}
```

欄位名 | 描述 
---------|----------
group | 小組
Ename | 姓名
Phone | 手機


<div><h1>回傳 JSON</h1></div>

```json
{
  "DataChangeMsg": [
    "原手機號碼 0919963322 是否變更為 「0919963327」",
    "原彥伯小組是否變更為「漢威小組」"
  ],
  "group": "CA202.信豪牧區-彥伯小組",
  "Ename": "劉彥伯",
  "Phone": "0919963327",
  "MID": "758",
  "ApiTitle": "您有變更手機號碼？",
  "IsChgShow": true
}
```

欄位名 | 描述 
---------|----------
DataChangeMsg | 資料變更訊息提醒(可以有多條訊息)
group | 小組
Ename | 姓名
Phone | 手機
MID | 會友流水編號
ApiTitle | 資料變更訊息的Title
IsChgShow | 若為true表示要show資料變更頁面, 若為false表示直接呼叫 Api\AddSubSign show 報名結果頁面