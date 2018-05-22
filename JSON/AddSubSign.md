<div><h1>傳入 JSON</h1></div>

```json
{
  "SID": 1,
  "CategoryID": "C1",
  "gcroup": "社青",
  "group": "CA202.信豪牧區-彥伯小組",
  "Ename": "Test",
  "Phone": "0919123456"
}
```

欄位名 | 描述 
---------|----------
SID | API\GetSUBInfo.aspx 回傳的課程id編號
CategoryID | 網旨的id參數  http://changelifesys.org/SubjectSignUp.aspx?id=c1
gcroup | 組別
group | 小組
Ename | 姓名
Phone | 手機


<div><h1>回傳 JSON</h1></div>

```json
{
  "CategoryID": "C1",
  "SID": 1,
  "gcroup": "社青",
  "group": "CA202.信豪牧區-彥伯小組",
  "Ename": "Test",
  "Phone": "0919123456",
  "Gmail": "",
  "Church": "",
  "ApiMsg": "",
  "IsApiError": false
}
```

欄位名 | 描述 
---------|----------
CategoryID | 傳入網旨的id參數(http://changelifesys.org/SubjectSignUp.aspx?id=c1)
SID | 回傳課程id編號
gcroup | 組別
group | 小組
Ename | 姓名
Phone | 手機
Gmail | 保留欄位, 固定回傳空值
Church | 保留欄位, 固定回傳空值
ApiMsg | API的訊息, 若IsApiError=true則顯示該訊息, 資料正常就為 null。
IsApiError | IsApiError=true 表示API有錯誤; IsApiError=false 表示API無誤。
