<div><h1>API ChkMember</h1></div>

API | 描述 
---------|----------
用途說明 | 驗證會友填入的資料
使用位置 | SubjectCheck.aspx 課程簽到, SubjectSignUp.aspx 課程報名

<div><h1>傳入 JSON</h1></div>

```json
{
  "group": "CA202.信豪牧區-彥伯小組",
  "Ename": "劉彥伯",
  "Phone": "0919963322",
  "SID": 1
}
```

欄位名 | 描述 
---------|----------
group | 小組
Ename | 姓名
Phone | 手機
SID | 課程id編號

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
  "IsChgShow": true,
  "SID": 1
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
SID | 課程id編號