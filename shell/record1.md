#Linux下一行执行多条命令的三种方式
##1.使用&&连接符
&&连接符的作用是只有前面一条命令执行成功后，才会执行后面的一条命令
###例子
>mkdir testdir && cd testdir

##2.使用||连接符
||连接符的作用是只有前面一条命令执行失败后，才会执行后面一条命令
>mv testdir testdir2 || echo "hello world"

##3.使用；连接符
；连接符的作用是顺序执行多条命令，前面一条命令执行后，不管其执行结果如何，都会继续执行后面一条命令
>mv testdir testdir3 || echo "hello world"

