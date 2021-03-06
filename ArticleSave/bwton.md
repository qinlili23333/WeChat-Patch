# 实锤某毒瘤公司所开发的APP的流氓行为
## 某公司说我恶意抹黑拿不出证据，那我今天倒是要把这个一年前的回答好好补充全证据！

## 明天就考试，但我就不复习！就是要和毒瘤对抗到底！

## 本文一切内容真实可复现！如果你复现不出来请告诉我你的设备环境，我会尽可能协助你复现结果

由于我是苏州人，我就取这家毒瘤公司为苏州地铁开发的app做例子吧

我们从[苏e行-小米应用商店](https://link.zhihu.com/?target=https%3A//app.xiaomi.com/details%3Fid%3Dcom.bwton.szfreego)下载安装包，并截图小米商店网页的版本号和更新时间

![](https://pic2.zhimg.com/v2-21a13a9811046d2b950ce24dbab27b51_b.jpg)

![](https://pic2.zhimg.com/80/v2-21a13a9811046d2b950ce24dbab27b51_1440w.jpg)

  

得到58.42M安装包一个

![](https://pic2.zhimg.com/v2-40dcd3f0cd6bf7852158890d93db40e5_b.jpg)

![](https://pic2.zhimg.com/80/v2-40dcd3f0cd6bf7852158890d93db40e5_1440w.jpg)

记录文件校验，以确保这是一个完整的文件，

![](https://pic4.zhimg.com/v2-11057fb70b8852afdeb058a7c54db46b_b.jpg)

![](https://pic4.zhimg.com/80/v2-11057fb70b8852afdeb058a7c54db46b_1440w.jpg)

为了确保没有任何其他APP干扰，我准备了一个全新的炼妖壶环境，可以看到炼妖壶里除了系统必须的谷歌套件外只有一个mt管理器，而且存储空间内啥也没有非常干净

![](https://pic2.zhimg.com/v2-aa3e80d7bbdff3ab7db40d00b7626cf9_b.jpg)

![](https://pic2.zhimg.com/80/v2-aa3e80d7bbdff3ab7db40d00b7626cf9_1440w.jpg)

  

![](https://pic2.zhimg.com/v2-31307ffa05b7db26d4b70d322851c751_b.jpg)

![](https://pic2.zhimg.com/80/v2-31307ffa05b7db26d4b70d322851c751_1440w.jpg)

我们把安装包安装到炼妖壶

![](https://pic2.zhimg.com/v2-d694a2be8dd09231323ea3eaee0c7549_b.jpg)

![](https://pic2.zhimg.com/80/v2-d694a2be8dd09231323ea3eaee0c7549_1440w.jpg)

  

## 证明环节1：滥用权限

直接打开app，同意用户协议，但拒绝电话和文件权限请求（这个app用来刷地铁，显然这两个权限和该app必须功能没有任何关联）

![](https://pic1.zhimg.com/v2-2cd9e79625314f1ebe94dcb15dd25bac_b.jpg)

![](https://pic1.zhimg.com/80/v2-2cd9e79625314f1ebe94dcb15dd25bac_1440w.jpg)

ps：非常有意思的是，进入主界面后的位置权限拒绝了没什么后果

可明明位置权限倒是比电话权限有用114514倍啊

## 证明环节2：滥用后台

我们同意权限（反正壶中界，非常安全），进入app，过掉开屏后直接按下桌面按钮

可以看到弹出了该app在后台运行的toast

![](https://pic2.zhimg.com/v2-640f1d6d008c9b6d9b55faca523975c1_b.jpg)

![](https://pic2.zhimg.com/80/v2-640f1d6d008c9b6d9b55faca523975c1_1440w.jpg)

当然，可能有人要问了，我就弹个toast不能充分证明我在后台运行啊

所以在进入后台后，我打开终端

![](https://pic4.zhimg.com/v2-046d76fd2471a45a367f9f83da6b5dd7_b.jpg)

![](https://pic4.zhimg.com/80/v2-046d76fd2471a45a367f9f83da6b5dd7_1440w.jpg)

用top命令查看cpu占用，发现占用了2.3%（top只显示单核cpu占用，即占用一个核心的2.3%，和windows端任务管理器显示的全核占用有所区别请特别留意）

可能还有人会问，刚切入后台当然有占用，那么我们过几分钟去设置里看看

正常返回桌面5分钟左右之后我们打开该app设置页面的电池页面

![](https://pic2.zhimg.com/v2-2a0253a96cb4c9e6a85f7924d3e2d6f1_b.jpg)

![](https://pic2.zhimg.com/80/v2-2a0253a96cb4c9e6a85f7924d3e2d6f1_1440w.jpg)

足足运行了两分钟才被系统休眠（我系统设置全部禁止自启动禁止后台活动），显然是做了保活的

你一个刷地铁的app，有什么后台存活需求么？进出站刷一下不就够了？

## 证明环节3：全包加固

![](https://pic3.zhimg.com/v2-971e65ed63ead409675d8b53bef7e422_b.jpg)

![](https://pic3.zhimg.com/80/v2-971e65ed63ead409675d8b53bef7e422_1440w.jpg)

##   

![](https://pic2.zhimg.com/v2-aa3b0b1a69956cf3dfaa4deff0036585_b.jpg)

![](https://pic2.zhimg.com/80/v2-aa3b0b1a69956cf3dfaa4deff0036585_1440w.jpg)

之前写那个回答的时候还是360加固，现在改用网易了

nesec.so，非常典型的网易加固，没法洗

## 证明环节4：32位

![](https://pic3.zhimg.com/v2-e4905fbb64f3181b7895b6dc1461ba22_b.jpg)

![](https://pic3.zhimg.com/80/v2-e4905fbb64f3181b7895b6dc1461ba22_1440w.jpg)

armeabi，铁32位，还tm是没neon的v5时代，山顶洞人么？

我检查过所有so文件了，都有对应64位sdk可以接入，没屎坑问题，那就是单纯的坏了

当然你硬要举例哪里上64位有屎坑难度尽管告诉我，我能解决的屎坑实在不行你交给我解决

## 证明环节5：X5 Webview

公共存储data目录，圈红均为实锤X5证据

![](https://pic4.zhimg.com/v2-f7740685b4cce5eaeaa0ec401a4f1f3f_b.jpg)

![](https://pic4.zhimg.com/80/v2-f7740685b4cce5eaeaa0ec401a4f1f3f_1440w.jpg)

还有这个service，洗不了

![](https://pic4.zhimg.com/v2-f9c06df3dc835fa14f35f34dc7d87363_b.jpg)

![](https://pic4.zhimg.com/80/v2-f9c06df3dc835fa14f35f34dc7d87363_1440w.jpg)

## 证明环节6：存储脱粪+证明环节7：使用个推推送

原本干净的壶中界，多了好多东西呢！

![](https://pic3.zhimg.com/v2-e1802379a2f42956582be7378f539d5a_b.jpg)

![](https://pic3.zhimg.com/80/v2-e1802379a2f42956582be7378f539d5a_1440w.jpg)

.tbs，QQBrowser，tencent都是接入X5带来的

turingdebug似乎也是X5的锅

bwtCashierSDK和bwton是这个app自己脱粪的，理应放在私有data目录

libs是个推SDK，个推老毒瘤SDK了这个libs文件斩草不除根春风吹又生，知乎也有，所以我现在禁止知乎写入存储

![](https://pic1.zhimg.com/v2-7d24814d0ebc40c08751107686dc1934_b.jpg)

![](https://pic1.zhimg.com/80/v2-7d24814d0ebc40c08751107686dc1934_1440w.jpg)

加起来体积不大，但是污染公共存储确实是毒瘤行为

**所有不需要共享的数据，请务必存储于data目录，为了存储整洁，也为了数据安全**

## 表扬时间

一个一年前发现但当前已被修补的问题是SDK版本过低，当时不同的app分别为22或26，目前已被提升到28，该表扬的我也绝对不会少表扬，但是目前最新的应该是30咯！

![](https://pic2.zhimg.com/v2-4be96f3978008bbb2eeb169dfcfee421_b.jpg)

![](https://pic2.zhimg.com/80/v2-4be96f3978008bbb2eeb169dfcfee421_1440w.jpg)

## 总结

一年前写的回答到此已全部给出充分证据实锤

如果该公司仍然认为我是在恶意抹黑请拿出充分证据，如果该公司坚持我是同行，那也请拿出充分证据

## 本文全部证据均使用合法的工具软件取得，没有通过任何反编译手段进行

## 我的证据列完了，请反击或认输，我愿意奉陪到底

## 我不是该行业从事人员，我只不过是个学制药的大二学生，我对科技和程序只不过是兴趣爱好罢了，但我仍然坚持为更美好的软件生态贡献自己的力量

  

##   

## 小彩蛋

经典打包事故，把网易加固的SDK jar文件也给打包进去了，还有那个aapt文件夹也不用打包

![](https://pic4.zhimg.com/v2-e091f36a1358898e4dab450776c6a89b_b.jpg)

![](https://pic4.zhimg.com/80/v2-e091f36a1358898e4dab450776c6a89b_1440w.jpg)

## 本文Copyleft,你可以随意转载并用你想用的任何身份发表
