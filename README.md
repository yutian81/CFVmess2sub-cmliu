## 手动订阅器生成自定义订阅
> 这里以CMLiu的订阅器为例  
> 实际使用时请去掉`[ ]`符号，Worker部署优先使用自定义域！！！  

### Trojan自定义订阅
- pages部署
```
https://Trojan.fxxk.dedyn.io/sub?host=[你的Trojan域名]&pw=[你的password]&path=[你的ws路径]
```
- Worker部署
```
https://Trojan.fxxk.dedyn.io/sub?host=[你的Worker域名]&pw=[你的password]
```

### VLESS自定义订阅
- pages部署
```
https://VLESS.fxxk.dedyn.io/sub?host=[你的VLESS域名]&uuid=[你的UUID]&path=[你的ws路径]
```
- Worker部署
```
https://VLESS.fxxk.dedyn.io/sub?host=[你的Worker域名]&uuid=[你的UUID]
```

### VMESS自定义订阅
- 完整格式
```
https://VMess.fxxk.dedyn.io/sub?cc=[VMess服务名字]&host=[你的VMess域名]&uuid=[你的UUID]&path=[你的ws路径]&alterid=[额外ID]&security=[加密方式]
```
  *cc 非必填项，可能会影响使用在线订阅转换,推荐使用地区代号，例如HK、SG、US*  
  *alterid 非必填项，默认0*  
  *security 非必填项，默认auto*  
- 精简格式
```
https://VMess.fxxk.dedyn.io/sub?host=[你的VMess域名]&uuid=[你的UUID]&path=[你的ws路径]
```

### WARP自定义订阅
- 格式一：优选ip+端口
```
https://WARP.fxxk.dedyn.io/sub?ip=[优选ip:端口]
```
例如：`https://WARP.fxxk.dedyn.io/sub?ip=162.159.195.179:987`
- 格式二：优选IP.txt文件地址
```
https://WARP.fxxk.dedyn.io/sub?api=[优选IP.txt文件地址]
```
例如：`https://WARP.fxxk.dedyn.io/sub?api=https://raw.githubusercontent.com/cmliu/WARP2sub/main/ip.txt`
- 格式三：优选测速csv文件地址
```
https://WARP.fxxk.dedyn.io/sub??csv=[优选结果csv文件地址]
```
例如：`https://WARP.fxxk.dedyn.io/sub?csv=https://raw.githubusercontent.com/cmliu/WARP2sub/main/result.csv`
- 格式四：PrivateKey私钥
```
https://WARP.fxxk.dedyn.io/sub?key=[PrivateKey私钥]
```
例如：`https://WARP.fxxk.dedyn.io/sub?key=iNw48fdfcf4wrc9i7A21gyFG09a3E3NPydvb2ysTQGY=`
