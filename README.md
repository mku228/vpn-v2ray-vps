# 海外云服务vps机场一键安装v2ray加速bbr(图文傻瓜式最新教程)

## 原理简介
如今大的机场都改用了trojan/v2ray协议，抛弃了易被封锁的ss协议。ws+tls或ws+tls+caddy经受住了考验，目前比较稳定。

Linux服务器系统有两种主流的网络加速算法。其中，serverSpeeder是中国华夏创新公司的付费产品，惨遭国人破解。谷歌公司免费的BBR tcp堵塞优化算法，已经集成在最新版本的Linux内核，免费使用。锐速逐渐被淘汰。

## 优惠获取海外vps

一台海外服务器是必需条件。如果你是新手，建议[购买Vultr服务器](https://github.com/mku228/vultr-signup-zh-tutorial)，付款方式有信用卡、支付宝和微信，新用户送100美元优惠码。([你可以点击 vultr 专属赠送新用户 100 美元 进去抢先注册。](https://www.vultr.com/?ref=8944093-8H))

注册创建教程：[Vultr服务器注册和创建教程](https://github.com/mku228/vultr-signup-zh-tutorial)

通过以上教程你已经获取了一台服务器，并且连接上了。

## v2ray 搭建教程

### 1.避免VPS没装Curl，保险起见运行一下 Curl的安装命令, 两种系统下随便用一个命令就可以。

ubuntu/debian 系统下 ：

```
apt-get install curl -y
```

![image](https://user-images.githubusercontent.com/98797623/152306980-daaa0a4f-396a-452a-9bea-69cb5b131417.png)

centos 系统下:

```
yum install curl -y
```

### 2.一件脚本安装v2ray

```
bash <(curl -s -L https://git.io/v2ray.sh)
```

粘贴后，Enter， 进入下列菜单
输入 1 按 Enter 继续

![image](https://user-images.githubusercontent.com/98797623/152307333-bd6e2a5e-cda9-4b11-ab17-04edcb8d3d81.png)

V2Ray的功能比较多，我们不用管
看到以下界面直接按 Enter 继续

![image](https://user-images.githubusercontent.com/98797623/152307376-dc8806f0-4034-43f1-b247-bbf833b6c232.png)

继续 Enter

![image](https://user-images.githubusercontent.com/98797623/152307418-cab764e8-d899-4687-84a5-9ad6570e3f64.png)

继续 Enter

![image](https://user-images.githubusercontent.com/98797623/152307447-986fa971-4036-4d81-8447-8173bf95288d.png)

继续 Enter:

![image](https://user-images.githubusercontent.com/98797623/152307491-78da8167-e2a9-40a8-ade0-2d49e8223ebb.png)

还是Enter:

![image](https://user-images.githubusercontent.com/98797623/152307533-fa944237-a747-4cff-9018-a6021807464f.png)

等个几十秒

### 3. 看到如下界面之后 

输入 v2ray url 复制出来 Vmess Url 【选中后用鼠标右键复制】

![image](https://user-images.githubusercontent.com/98797623/152307603-978bf299-01d0-411f-a025-81de0506d80c.png)

复制黄色区域 / 鼠标右键复制

![image](https://user-images.githubusercontent.com/98797623/152307633-abf6d1ee-4934-423b-8b0a-3cd9da888929.png)


## V2ray 的连接 【以Windows为例]

下载 V2ray 软件: https://github.com/2dust/v2rayN/releases
下载 v2rayN-Core.zip 到桌面解压
打开 V2rayN 程序

![image](https://user-images.githubusercontent.com/98797623/152307752-8f2243a4-87b6-43a7-ac88-ba7d0f05d16f.png)

添加 Vmess 服务器

![image](https://user-images.githubusercontent.com/98797623/152307786-49a06c1a-8883-495a-86fc-f18e0d85204f.png)

复制刚才复制的代码 Vmess地址
我把这个共享在 Free SS 资源 有需要的直接拿来用，也可以用来测试下速度
从剪切板导入URL ； 点确定

![image](https://user-images.githubusercontent.com/98797623/152307828-de636189-acfb-4c8f-9998-44306742b576.png)

回到V2ray 主界面，这里多了一个 新的服务器

![image](https://user-images.githubusercontent.com/98797623/152307857-92a382f5-5b70-4eab-91ed-ea3e0f15dd7e.png)

参数设置 2333
点确定

![image](https://user-images.githubusercontent.com/98797623/152307925-e7a0dea3-2040-443c-af9a-45f7af2378c8.png)

右键点图标启用即可，
有风险提示，就点允许

![image](https://user-images.githubusercontent.com/98797623/152307958-1ed0b5c3-dc7b-4587-826c-65325585a873.png)


连接完成:

![google](https://user-images.githubusercontent.com/98797623/152308005-a7e283c8-4782-4591-8bbd-58184522e3fa.png)



















