# pdown
---
百度网盘下载器，2020,百度网盘高速下载
> PDown是个人项目，开始是作为毕业设计立项，为了方便宿舍下载试验资料。 现在分享出来希望可以帮助到更多的人

![demo](down600.gif)


#### [蓝奏云 4-4 22:21 下载地址  https://pdown.lanzous.com/ib00pof](https://pdown.lanzous.com/ib00pof)
---
### 0.项目刚发布，确实有不少BUG，请参阅 [更新日志.md](更新日志.md)  
最新更新时间：2020-4-4 22:21，近期我们更新很频繁的。如果遇到各种不能下载/无限拉取，请多包容，过一天再试BUG可能就被修复了，请留意我们的版本更新。过一个月程序就稳定了，就不会有频繁的版本更新了<br/><br/>

#### 3月28日我已调整单个文件体积最大100MB，链接内所有文件的总体积最大500MB，请见谅。PDown的初衷只是方便大家临时应急用用而已

### 1.安装使用

软件是单文件.exe(**5MB**) 无需安装,下载后双击直接运行<br/>
直接粘贴  **完整的**  百度分享链接和**提取码**，就可以下载了。不需要登录你的百度账号<br/>
总有人只粘贴分享链接不包括提取码, 应该像这样粘贴完整的链接+提取码<br/>
```
链接：https://pan.baidu.com/s/1jxP5vznx3_XvHrPKv1yhKg 提取码：97zc 
```

### 2.加速原理

你提交链接  -->  我去下载  -->  我传给你<br/><br/>
所以可能你的任务会长时间一直在拉取（尤其是大文件），要耐心等着

### 3.加速效果

个人免费项目，没钱开很多服务器+宽带。所以有很多的限制，正常情况下限速300kb/s / 最多3文件同时下载<br/>
<del>你可以在软件里使用手机登录，登录后限速为600kb/s / 最多3文件同时下载</del><br/>
有特殊情况:<br/>
* 同时使用的人很多时，要排队拉取，你需要等待很长时间，才能拉取成功<br/>
* 有的文件使用 百度客户端下载也很慢，甚至不能下载，应该是百度CDN调度问题 ( 还比较常见 )<br/>
* 只支持包含小文件的分享链接， 单个文件体积<100MB ,链接内所有文件的总体积<500MB （因为大文件会导致其他人长时间等待）<br/><br/>

<br/><br/>
   
现在只是测试阶段，拉取可能需要多等等。总之一句话，自己使用一下才知道。<br/>
  
 3月28日备注：
> 项目上线10天了，今天服务器又被挤爆了，个人项目财力有限，我确实没有预料到会有这么多人用  
> 最近几天都是，一个任务基本需要等待半小时以上的拉取。技术上我已经优化的很好了，但架不住排队的人多  
> 现在看拉取超半小时，已经完全失去了使用PDown的意义了。我被迫又一次下调了文件体积限制，别骂我，我尽力了  
>  
> Ps1:调整的原因是拉取小文件速度很快，大家可以提交链接后很快就开始下载，100MB足够小了，以后不会再胡乱调整  
> Ps2:调整只涉及新增链接，调整前已提交的链接我都会努力帮你们完成下载，不受影响。等以后用的人少了，我会调回来  
> Ps3:跟所有人说声抱歉，是我阅历太少能力不够，太想当然了

---

#### Q:什么时候会收费？
个人项目，永久免费。没钱我会去寻求捐赠，实在没钱我会关掉项目。所以永远免费。
#### Q:文件版权纠纷?
我一直在监管版权问题，并且提供了醒目的举报入口，欢迎大家和我们一起维护版权，打击各种违规文件。只要举报无条件封杀<br/>  
因为只有小文件（电影什么的不可能有），加上是个人项目并没有很多人在用。实际上也很难有所谓版权纠纷。<br/>
但如果确实涉及到您的版权请及时联系我。我会立即清理<br/><br/>
#### Q:有问题怎么联系？
github上发Issue吧，我会不定时的来看看的，看到了就会回复你
#### Q:会开源吗？用的什么技术？
客户端是c++，用到了SOUI3，SQLite，Curl，GoogleBase，等等，界面都是我自己设计后用PS贴图<br/>
具体的代码因为是个人项目，又乱又杂，还有一堆BUG。实在羞于出手。等以后项目稳定了会考虑开源客户端的部分代码，因为SOUI就是开源的<br/>
