<div><h1>傳入 JSON</h1></div>

```json
{
  "SID": "1",
  "CategoryID": "C1",
  "gcroup": "社青",
  "group": "CA202.信豪牧區-彥伯小組",
  "Ename": "Test",
  "Phone": "0919123456"
}
```

欄位名 | 描述 
---------|----------
SID | 回傳的課程id編號
CategoryID | 傳入網旨的id參數(http://changelifesys.org/SubjectSignUp.aspx?id=c1)
gcroup | 下拉選單的「組別」
group | 下拉選單的「小組」
Ename | 姓名
Phone | 手機


<div><h1>回傳 JSON</h1></div>

```json
{
  "CategoryID": "C1",
  "SID": 1,
  "SubName": "生命建造程序 C1 課程報名",
  "SUCondition": "2018年1月~2018年12月來的新朋友，或是還沒上過的會友。",
  "SubDate": "5/5 上午 12:00:00(六) 下午 14:30~17:30",
  "SubLocation": "江子翠行道會主會堂",
  "SubEndDate": "即日起~5/31 上午 12:00:00(四) 截止報名，之後請現場報名。",
  "ApiMsg": null,
  "IsApiError": false
}
```

欄位名 | 描述 
---------|----------
CategoryID | 傳入網旨的id參數(http://changelifesys.org/SubjectSignUp.aspx?id=c1)
SID | 回傳課程id編號
SubName | 對應標題字串「生命建造程序 C1課程報名」
SUCondition | 對應報名條件「2016年12月~2017年2月來的新朋友，或是還沒上過的會友。」
SubDate | 對應上課日期「2/12(日)、 2/19(日)下午14:30~17:30」
SubLocation | 對應地點「江子翠行道會主會堂」
SubEndDate | 對應報名日期「即日起~2/9(四)截止報名，之後請現場報名。」
ApiMsg | API的訊息, 若IsApiError=true則顯示該訊息, 資料正常就為 null。
IsApiError | IsApiError=true 表示API有錯誤; IsApiError=false 表示API無誤。
