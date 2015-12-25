---
layout: module
title: Module 2&#58; Starting the Node Server
---
In this module, you install and start a Node.js server that exposes the conference data (sessions and speakers) 
through a set of REST services.

## Steps

1. 使用 [git] (https://git-scm.com/) clone 指令，或者到[原著作的github](https://github.com/ccoenraets/ionic-tutorial/archive/master.zip)下載:

    ```
    git clone https://github.com/ccoenraets/ionic-tutorial
    ```

    > 
D:\ionic>git clone https://github.com/ccoenraets/ionic-tutorial
    > 
  Cloning into 'ionic-tutorial'...
    > 
remote: Counting objects: 2690, done.
    > 
remote: Total 2690 (delta 0), reused 0 (delta 0), pack-reused 2690
    > 
Receiving objects: 100% (2690/2690), 11.52 MiB | 1.86 MiB/s, done.
    > 
Resolving deltas: 100% (779/779), done.
    > 
Checking connectivity... done.
    > 
>
D:\ionic>

1. 在命令行模式進入 **ionic-tutorial/server** 目錄
 
    ```
    cd ionic-tutorial
    cd server
    ```


1. 安裝 server dependencies:

    ```
    npm install
    ```

1. 啟動 node server:

    ```
    node server
    ```
  
    > 如果有錯誤，察看是否有其它 server 已在監聽 port 5000.

1. 測試 REST services. 打開流覽器訪問:
    - [http://localhost:5000/sessions](http://localhost:5000/sessions) (for a list of conference sessions returned as a JSON document)
    - [http://localhost:5000/sessions/1](http://localhost:5000/sessions/1) (for information about a specific session )
  

<div class="row" style="margin-top:40px;">
<div class="col-sm-12">
<a href="install-ionic.html" class="btn btn-default"><i class="glyphicon glyphicon-chevron-left"></i> 
Previous</a>
<a href="create-ionic-application.html" class="btn btn-default pull-right">Next <i class="glyphicon 
glyphicon-chevron-right"></i></a>
</div>
</div>


