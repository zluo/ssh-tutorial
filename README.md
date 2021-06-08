SSH 是 Linux 系统的登录工具，现在广泛用于服务器登录和各种加密通信。

本教程介绍 SSH（主要是它的实现 OpenSSH）的概念和基本用法，也可以当作手册查询。


##Generate html with Loppo 

Loppo is an extremely easy static site generator of markdown documents. You get your site with only one command. Please visit demo.

###Features

 easy config (example)

. simple site structure (example)
friendly template syntax(example)
built-in utility commands

###How to use

First of all, arrange your documents into the following structure.

|- myProject
|- README.md
|- docs
|- page1.md
|- page2.md
|- ...

Now, install Loppo.

    $ npm install loppo -g

Enter your project directory.

    $ cd myProject
Run the command.

    $ loppo
Now, Loppo will build the document site under dist sub-directory. After the building process, you could open the site in your browser.

    $ open dist/index.html


=== Setup Home Page
. install apache

. add host name to /etc/host

    my 127.0.0.1

. create softlink to /var/www/html

    cd /var/www/html
    sudo ln -s /home/zluo/src/lab/ssh-tutorial/dist/ ssh-tutorial