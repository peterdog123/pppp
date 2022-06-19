|合約1:|click sign in()|
|操作:|click sign in()|
|交互參照:|登入|
|前置條件:|已註冊帳號|
|後置條件:|-跟資料庫驗證帳號verify account()<br>-回報登入結果return login result()|

|合約2:|verify account()|
|操作:|verify account()|
|交互參照:|登入帳號|
|前置條件:|已註冊帳號|
|後置條件:|-回報登入結果return login result()|

|合約3:|fill in the basic information()|
|操作:|fill in the basic information()|
|交互參照:|填寫基本資料作業|
|前置條件:|已經登入成功|
|後置條件:|傳送給資料庫passToDatabase(name,home,number)|

|合約4:|pass to database()|
|操作:|pass to database(name,number,address)|
|交互參照:|填寫基本資料作業|
|前置條件:|已經登入成功|
|後置條件:|回報註冊結果report access complete()|

|合約5:|add focus on TikToker()|
|操作:|add focus on TikToker()|
|交互參照:|關注TikToker|
|前置條件:|已經登入成功|
|後置條件:|顯示TikToker內容show TikTokor content()|

|合約6:|send gift()|
|操作:|send gift()|
|交互參照:|關注TikToker|
|前置條件:|已經送出禮物|
|後置條件:|傳送給資料庫send to database()<br>-回傳結果report access complete()|

|合約7:|report problem()|
|操作:|report problem()|
|交互參照:|聯絡客服作業|
|前置條件:|操作有問題|
|後置條件:|客服中心要回復使用者reply to the user()|

|合約8:|logout of the system()|
|操作:|logout of the system()|
|交互參照:|登出作業|
|前置條件:|離開網頁|
|後置條件:|跳出登出訊息show logout message()|


|合約9:|reception problem()|
|操作:|reception problem()|
|交互參照:|客服解決問題作業|
|前置條件:|登入系統|
|後置條件:|解決使用者問題problem solved()|

|合約10:|check system()|
|操作:|check system()|
|交互參照:|維護網站作業|
|前置條件:|登入後台|
|後置條件:|定時檢查網頁與後台check web and backstage()|