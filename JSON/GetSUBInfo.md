<div><h1>API GetSUBInfo</h1></div>

API | 描述 
---------|----------
用途說明 | 取得課程資訊
使用位置 | SubjectCheck.aspx 課程簽到, SubjectSignUp.aspx 課程報名


<div><h1>傳入 JSON</h1></div>

```json
{
  "CategoryID": "C1"
}
```

欄位名 | 描述 
---------|----------
CategoryID | 傳入網旨的id參數(http://changelifesys.org/SubjectSignUp.aspx?id=c1)


<div><h1>回傳 JSON</h1></div>

```json
{
  "CategoryID": "C1",
  "SID": 1,
  "SubName": "生命建造程序 C1 課程報名",
  "ApiMsg": "",
  "IsApiError": false,
  "HtmlSubDesc": "<div class='class-info'><div role='alert' class='el-alert el-alert--info'><!----><div class='el-alert__content'><!----><p class='el-alert__description'>本表個人資料將作建檔處理，並於日後會務活動運作之目的內，由教會及同工作為聯絡通訊、關懷及相關合理運用。我們會盡善良管理人責任，妥善保管資料，避免外洩或不當用途之使用。</p><i class='el-alert__closebtn el-icon-close' style='display: none;'></i></div></div><ul class='class-detail'><li><div class='class-detail-title'>報名條件：</div><div class='class-detail-text'>2018年1月~2018年12月來的新朋友，或是還沒上過的會友。</div></li><li><div class='class-detail-title'>上課日期：</div><div class='class-detail-text'>08/05(日)、08/12(日) 下午 14:30~17:30</div></li><li><div class='class-detail-title'>地點：</div><div class='class-detail-text'>江子翠行道會主會堂</div></li><li><div class='class-detail-title'>報名日期：</div><div class='class-detail-text'>即日起~07/31(二) 截止報名，之後請現場報名。</div></li></ul></div>"
}
```

欄位名 | 描述 
---------|----------
CategoryID | 傳入網旨的id參數(http://changelifesys.org/SubjectSignUp.aspx?id=c1)
SID | 回傳課程id編號
SubName | 對應標題字串「生命建造程序 C1課程報名」
ApiMsg | API的訊息, 若IsApiError=true則顯示該訊息, 資料正常就為空值。
IsApiError | IsApiError=true 表示API有錯誤; IsApiError=false 表示API無誤。若有錯誤則alert出ApiMsg欄位的訊息，且不讓user填資料。
HtmlSubDesc | 課程內容
