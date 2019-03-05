### 修改bash，配置自定义命令
```
vi ~/.bash_profile
```
### 在文件结尾增加以下配置
```
alias proxy='export all_proxy=socks5://127.0.0.1:1080'
alias unproxy='unset all_proxy'
```

### 使配置生效
```
source ~/.bash_profile
```

### 开启配置
```
proxy
```

### 关闭配置
```
unproxy
```

### 配置验证
```
curl ipinfo.io
```

