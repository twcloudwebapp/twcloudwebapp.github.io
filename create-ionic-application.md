---
layout: module
title: 第三課&#58; 新建 Ionic APP
---
使用命令行 CLI (command line interface) 新建具有 sidemenu 模板的 APP。 


## 步驟

1. Open a new terminal window (Mac) or a command window (Windows), and navigate (cd) to the **ionic-tutorial** directory

1. Using the Ionic CLI, create an application named **conference** based on the **sidemenu** starter app:

    ```
    ionic start conference sidemenu
    ```

1. Navigate to the **conference** folder 

    ```
    cd conference
    ```

1. Start the application in a browser using **ionic serve**.

    ```
    ionic serve
    ```

    會在網頁上出現 iOS 和 Android 查看這網站的模樣，

    ```
    ionic serve --lab
    ```

    > NOTE: 直接打開網頁得不到應有的效果，必需有 web server。**ionic serve** 是個本地端輕量級的 web server，隨著程式碼改變，不必人為去按F5刷新，能立即自動重載更新。

1. In the application, open the side menu ("hamburger" icon in the upper left corner) and select 
**Playlists**. 
Select a playlist in the list to see the details view (not much to see at this point).

    In the next modules, you will replace the playlists with a list of conference sessions retrieved from the 
    server using the REST services you experimented with in the previous module.

1. Open the side menu again and select **Login**. Click the Login button to close the window (Login is not 
implemented in the starter app).

    In the last module of this tutorial you will implement Login using **Facebook**.

<div class="row" style="margin-top:40px;">
<div class="col-sm-12">
<a href="start-node-server.html" class="btn btn-default"><i class="glyphicon glyphicon-chevron-left"></i> 
上一課</a>
<a href="create-angular-service.html" class="btn btn-default pull-right">下一課 <i class="glyphicon 
glyphicon-chevron-right"></i></a>
</div>
</div>