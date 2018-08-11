# node 8.6
#### image测试网速、上报数据</br>
* 利用image测网速
```
<body>
<div id="a"></div>
<script>
  let img = new Image()
  let date1 = Date.now()
  img.src = 'https://c565784135.gitee.io/pubilc/image/11.png'
  img.onload = function (e) {
    let date2 = Date.now()
    let kb = 4
    let s =  Math.round(kb / ((date2 - date1)/1000))
    document.getElementById('a').innerText = '你当前网速为'+s+'KB/S'
    
  }
</script>
</body>
```
* 通过小图访问记录用户行为（原理：通过web服务的access日志分析用户行为数据)
```
https://hm.baidu.com/hm.gif?cc=0&ck=1&cl=24-bit&ds=375x667&vl=667&et=0&ja=0&ln=zh-cn&lo=0&rnd=342377793&si=12423ecbc0e2ca965d84259063d35238&v=1.2.33&lv=1&ct=!!&tt=%E7%99%BE%E5%BA%A6%E4%B8%80%E4%B8%8B&sn=52245
```
#### css远程攻击漏洞</br>
#### iframe对远程localStroage扩容</br>
#### html语义化</br>
