<div><h1>API GetGroupItem</h1></div>

API | 描述 
---------|----------
用途說明 | 取得小組資訊
使用位置 | SubjectCheck.aspx 課程簽到, SubjectSignUp.aspx 課程報名, MemSubQuery.aspx 會友查詢, Exam.aspx 會友考試


<div><h1>傳入 JSON</h1></div>


```json
{
  "CategoryID": "C1"
}
```

欄位名 | 描述 
---------|----------
CategoryID | 傳入網旨的id參數(http://changelifesys.org/SubjectSignUp.aspx?id=c1),(http://changelifesys.org/SubjectCheck.aspx?id=c1)


<div><h1>回傳 JSON</h1></div>

```json
{
  "CategoryID": "C1",
  "DataInfo": [
    {
      "group": "家庭組弟兄",
      "list": [
        "AA101.永健牧區-永健小組",
        "AA102.永健牧區-本憲小組",
        "AA103.永健牧區-瑞嘉小組",
        ...
      ]
    },
    {
      "group": "家庭組姊妹",
      "list": [
        "BA101.佳琦牧區-雯閔小組",
        "BA102.佳琦牧區-若珊小組",
        "BA103.佳琦牧區-嘉玲小組",
        ...
      ]
    },
    {
      "group": "社青",
      "list": [
        "CA101.育仁牧區-祐嘉小組",
        "CA102.育仁牧區-璟佑小組",
        "CA103.育仁牧區-暉儒小組",
        ...
      ]
    },
    {
      "group": "學生",
      "list": [
        "EA101.大專冠綸牧區-樂研小組",
        "EA102.大專冠綸牧區-晧瑋小組",
        "EA103.大專冠綸牧區-綺珮小組",
        ...
      ]
    }
  ]
}
```

欄位名 | 描述 
---------|----------
CategoryID | 傳入網旨的id參數(http://changelifesys.org/SubjectSignUp.aspx?id=c1),(http://changelifesys.org/SubjectCheck.aspx?id=c1)
group | 組別
list | 小組