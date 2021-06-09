### 1. git 安装
```Shell
brew install git
```
### 2. 生成私钥
```Shell
ssh-keygen -t rsa -C "XXX@XXX.com"
```

```shell
Generating public/private rsa key pair.
Enter file in which to save the key (/Users/XXX/.ssh/id_rsa): 
Enter passphrase (empty for no passphrase): 
Enter same passphrase again: 
Your identification has been saved in /Users/XXX/.ssh/id_rsa.
Your public key has been saved in /Users/XXX/.ssh/id_rsa.pub.
The key fingerprint is:
SHA256:************ XXX@qq.com
The key's randomart image is:
+---[RSA 3072]----+
| o  .            |
|..+. o           |
|+...o.  .  .     |
|o.oo. .+. o      |
| =oo. +.So o     |
|o oo E o  o .    |
|.. .B o  . o     |
|. =oo* +  B      |
| o.+.o=.o+.o     |
+----[SHA256]-----+

```

### 3. cat 命令查看私钥内容并粘贴
```Shell
cat id_rsa.pub
```

### 4. 进入自己的GitHub主页并粘贴私钥
```shell
进入 SSH and GPG keys -> New SSH key
```


### 5. 验证是否成功
```shell
ssh -T git@github.com
```

### 6.成功后的提示
```shell
The authenticity of host 'github.com (52.74.223.119)' can't be established.
RSA key fingerprint is SHA256:nThbg6kXUpJWGl7E1IGOCspRomTxdCARLviKw6E5SY8.
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added 'github.com,52.74.223.119' (RSA) to the list of known hosts.
Enter passphrase for key '/Users/XXX/.ssh/id_rsa': 
Hi lifehrx! You've successfully authenticated, but GitHub does not provide shell access.
```