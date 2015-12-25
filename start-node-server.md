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

  Cloning into 'ionic-tutorial'...

remote: Counting objects: 2690, done.

remote: Total 2690 (delta 0), reused 0 (delta 0), pack-reused 2690

Receiving objects: 100% (2690/2690), 11.52 MiB | 1.86 MiB/s, done.

Resolving deltas: 100% (779/779), done.

Checking connectivity... done.


1. Open a terminal window (Mac) or a command window (Windows), and navigate (cd) to the **ionic-tutorial/server** 
directory

1. Install the server dependencies:

    ```
    npm install
    ```

1. Start the server:

    ```
    node server
    ```
  
    > If you get an error, make sure you don't have another server listening on port 5000.

1. Test the REST services. Open a browser and access the following URLs:
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


