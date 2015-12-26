---
layout: module
title: 第二課&#58; 啟動 Node Server
---

安裝並啟動 Node Server,透過 [REST](https://en.wikipedia.org/wiki/Representational_state_transfer) 提供研討會場次和演講者的信息。

為了擴展REST的部份，可以透過internet直接訪問，單獨在 [c9.io](https://c9.io/) 做，效果如下:

- [https://a01-twcloudwebapp.c9users.io:8080/sessions](https://a01-twcloudwebapp.c9users.io:8080/sessions) 

- [https://a01-twcloudwebapp.c9users.io:8080/sessions/1](https://a01-twcloudwebapp.c9users.io:8080/sessions/1) 



根據 [臺北市政府資訊局 市政網站整合平台之常見問答](http://data.taipei/opendata/datalist/datasetMeta?oid=203f1657-bb4a-45a7-b25f-279b63136645)

模仿前述的做法，在900多筆的情況還勉強可以接受，如何是再10倍或100倍以上的資料量時，就要有進一步的解決方案。

- [https://a01-twcloudwebapp.c9users.io:8080/taipeis](https://a01-twcloudwebapp.c9users.io:8080/taipeis) 

- [https://a01-twcloudwebapp.c9users.io:8080/taipeis/1](https://a01-twcloudwebapp.c9users.io:8080/taipeis/1) 




## 步驟

1. 使用 [git] (https://git-scm.com/) clone 指令:

    ```
    git clone https://github.com/ccoenraets/ionic-tutorial
    ```



1. 以 github 帳號 twcloudwebapp 註冊並登入 c9.io，新建 a01 project

1. 將 ionic-tutorial/server 裡的檔案複制到 a01
 
1. 安裝 package.json 裡的 server dependencies:

    ```
    twcloudwebapp:~/workspace $ npm install
    ```

1. 啟動 node server:

    ```
    twcloudwebapp:~/workspace $ node server
    Express server listening on port 8080
    ```
  
1. 新增**臺北市政府資訊局市政網站整合平台之常見問答**

- [Online XML to JSON](http://beautifytools.com/xml-to-json-converter.php)
- 在 routes 新增 taipeis
- 在 server.js 新增 

    ```
    app.get('/taipeis', taipeis.findAll);
    app.get('/taipeis/:id', taipeis.findById);
    ```

    

<div class="row" style="margin-top:40px;">
<div class="col-sm-12">
<a href="index.html" class="btn btn-default"><i class="glyphicon glyphicon-chevron-left"></i> 
上一課</a>
<a href="install-ionic.html" class="btn btn-default pull-right">下一課 <i class="glyphicon 
glyphicon-chevron-right"></i></a>
</div>
</div>


