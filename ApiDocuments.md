
## onCreated

### 生命周期-初始化

```javascript 
 
            $G.onCreated(()=>{
                console.log("onCreate");
            })
         
 ```

### 参数
> ##### 无需参数

### 返回值
> ##### 无返回值

---


## onShow

### 生命周期-进入前台

```javascript 
 
            $G.onShow(()=>{
                console.log("onShow");
            })
         
 ```

### 参数
> ##### 无需参数

### 返回值
> ##### 无返回值

---


## onHide

### 生命周期-进入后台

```javascript 
 
            $G.onHide(()=>{
                console.log("onHide");
            })
         
 ```

### 参数
> ##### 无需参数

### 返回值
> ##### 无返回值

---


## getSystemInfo

### 获取系统信息

```javascript 
 
            $G.getSystemInfo(
                success(info){
                    console.log(info)
                },
                fail(err){
                    console.log(err)
                }
            )
         
 ```

### 参数
> ##### 无需参数

### 返回值
> ##### buildVersion 说明 内部 build 版本 
> ##### appVersion 说明 webs app 的版本号 
> ##### appVersionNumber 说明 app内部版本，是一个累增的数字 
> ##### iosVersion 说明 ios的版本 
> ##### systemName 说明 设备名称 
> ##### model 说明 设备名称 
> ##### modelName 说明 手机型号 


---


## exitWebApp

### 退出当前程序

```javascript 
 
            $G.exitWebApp()
         
 ```

### 参数
> ##### 无需参数

### 返回值
> ##### 无返回值

---


## removeBackButton

### 移除返回按钮

```javascript 
 
            $G.removeBackButton()
         
 ```

### 参数
> ##### 无需参数

### 返回值
> ##### 无返回值

---


## removeViewTop

### 移除顶端的距离

```javascript 
 
            $G.removeViewTop()
         
 ```

### 参数
> ##### 无需参数

### 返回值
> ##### 无返回值

---


## addViewTop

### 增加顶端的距离

```javascript 
 
            $G.addViewTop()
         
 ```

### 参数
> ##### 无需参数

### 返回值
> ##### 无返回值

---


## setClipboard

### 设置粘贴板

```javascript 
 
            $G.setClipboard({
                data:new Date().getTime(),
                success(info){
                    console.log(info)
                },
                fail(err){
                    console.log(err)
                },
            });
         
 ```

### 参数
> ##### daya 说明 需要设置的文本 


### 返回值
> ##### 无返回值

---


## getClipboard

### 获取粘贴板

```javascript 
 
            $G.getClipboard({
                success(info){
                    console.log("info)
                },
                fail(err){
                    console.log(err)
                },
            });
         
 ```

### 参数
> ##### 无需参数

### 返回值
> ##### data 说明 获取粘贴板的文本 


---


## http

### 请求方法

```javascript 
 
            $G.http({
                headers:{
                    cookie:"device_id=317999456f5dcce56fd1ad7ef29c4f7d;"
                },
                method:"get",
                url:"http://xxxx.xxxx.com/xxx/xxx/xxxx/xxxxxxx.json",
                data:{
                    symbol:"SH000001",
                    begin:"1640533801003",
                    period:"year",
                    type:"before",
                    count:"-284",
                    indicator:"kline,pe,pb,ps,pcf,market_capital,agt,ggt,balance"
                },
                success(info){
                    console.log(info )
                },
                fail(err){
                    console.log(err)
                },
            })
         
 ```

### 参数
> ##### headers 说明 设置头文件 
> ##### method 说明 请求方式 
> ##### url 说明 请求链接 
> ##### data 说明 请求参数 


### 返回值
> ##### data 说明 返回值 
> ##### headers 说明 头信息 
> ##### statusCode 说明 状态码 
> ##### url 说明 请求链接 


---


## openUrl

### 打开外部方法

```javascript 
 
            $G.openUrl({
                url:"http://www.xxxxx.com",
                success(info){
                    console.log("info)
                },
                fail(err){
                    console.log(err)
                },
            });
         
 ```

### 参数
> ##### url 说明 需要打开的地址 


### 返回值
> ##### 无返回值

---


## setScreenOrientation

### 设置屏幕的方向

```javascript 
 
            // portrait 竖屏 
            // portraitUpsideDown 竖屏-相反方法 // 这个相仿方向不是固定的
            // landscapeLeft 横屏方向 - 左边
            // landscapeRight 竖屏  - 右边
            // all 所有方向 
            $G.setScreenOrientation({
                orientation:"portrait",
                success(info){
                    console.log("info)
                },
                fail(err){
                    console.log(err)
                },
            });
         
 ```

### 参数
> ##### orientation 说明 方向 


### 返回值
> ##### 无返回值

---

