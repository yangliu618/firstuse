# For first use git #

## step1. 生成git.corp的所需要的公钥,并上传 ##
<pre>
* sh-keygen -t rsa -C 'jackyang@anjuke.com'
* Generating public/private rsa key pair.
* Enter file in which to save the key (/home/yangliu/.ssh/id_rsa): gitcorp
* Enter passphrase (empty for no passphrase): 
* Enter same passphrase again: 
* Your identification has been saved in gitcorp.
* Your public key has been saved in gitcorp.pub.
* The key fingerprint is:
* 61:26:63:fa:d6:d2:d9:6b:3c:28:ff:1e:a3:39:d3:3c jackyang@anjuke.com
* The key's randomart image is:
* +--[ RSA 2048]----+
* |                 |
* |                 |
* |      + +        |
* |     o = .       |
* |    .   S        |
* |     . o o       |
* |      + +=+      |
* |     ...+oE+     |
* |       o+*+o     |
* +-----------------+
</pre>
    
把上面生成的gitcorp.pub的内容copy到git.corp上面进行授权.

## step2 git init ##

<pre>

 git clone git@git.corp.anjuke.com:yangliu/mygit
 git init
 git config user.name 'jackyang' #set username
 git config user.email 'jackyang@anjuke.com' #set email

</pre>

## step3 update you git ##

<pre>

>> vim test.php
>> git add .
>> git commit -m 'test' .
>> git push origin master:master

</pre>
