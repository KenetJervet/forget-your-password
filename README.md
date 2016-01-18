# forget-your-password
记住一个key，记住实体名，让程序为你生成密码。免除撞库攻击烦恼！


## 用法：

### 安装：

```bash
$ git clone https://github.com/KenetJervet/forget-your-password
$ cabal install
```

### 用法：

```bash
$ forget-your-password -h
Forget Your Password

Usage: forget-your-password unique-key salt [-l|--length password-length]
  Password generator

  Available options:
    -h,--help                Show this help text
    unique-key               Unique key
    salt                     Salt
    -l,--length password-length
			     Password length (1 ~ 32; Default is 8).
```

示例如下：

```bash
$ forget-your-password youtube.com jiangzemin
Your password is: sTtbELsY

$ forget-your-password youtube.com jiangzemin -l 16
Your password is: sTtbELsYyKJ4t4lG
```

好吧只是截断规则。。有点二逼么？我倒不觉得。。

死也不要把salt告诉别人！
