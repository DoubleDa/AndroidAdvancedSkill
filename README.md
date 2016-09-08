# Android进阶技能点

**目录**

## 1.RecyclerView


* [深入浅出RecyclerView(张涛)](http://kymjs.com/code/2016/07/10/01)

	介绍RecyclerView的基本用法、原理分析及其源码解析。

* [RecyclerView的通用适配器，和滚动时不加载图片的封装(张涛)](http://kymjs.com/code/2015/10/11/01)

	介绍RecyclerView的BaseAdapter、BaseViewHolder的封装，及滑动图片不加载。
	
* [那些酷炫的RecyclerView开源库整理](http://android.jobbole.com/83410/)

	最近在研究RecyclerView ，还是习惯整理一下开源项目放到github上 ，欢迎提交更新 ，fork，star。 排序纯属个人直觉。

* [Android LRecyclerView 实现下拉刷新，滑动到底部自动加载更多](http://android.jobbole.com/84060/)

	LRecyclerView是支持addHeaderView、 addFooterView、下拉刷新、分页加载数据的RecyclerView。

	它对 RecyclerView 控件进行了拓展，给RecyclerView增加HeaderView、FooterView，并且不需要对你的Adapter做任何修改。

* [十秒钟搞定RecyclerView数据绑定](http://gold.xitu.io/entry/575beb7e5bbb500053dbd451)

	在上一个项目里有很多很多很多很多的RecyclerView，然后我需要写很多很多很多很多的Adapter和Viewholder——多倒没问题，但是里面有很多重复的代码这就不能忍了！每一个Adapter和ViewHolder其实做的事情非常的像：视图绑定，数据绑定，点击事件分发。还有啥？既然它们做的事情都一样，为啥我们还要傻傻的继续写着重复的代码？

## 2.Android主题切换

* [Android夜间模式实现](http://kymjs.com/code/2015/05/26/01)

	介绍实现主题切换的简单实现思路，通过一个Demo进行讲解。

* [Android主题换肤的开源库ThemeSkinning](http://android.jobbole.com/83662/)

	本开源库是基于我之前的一个博客 Android主题换肤 无缝切换 不知道原理的可以去这篇博客看看。出于易于集成的目的，我将其抽取出来，作为一个模块。提供简洁的api，方便使用。
	
* [Android主题换肤无缝切换](http://android.jobbole.com/82932/)

	今天再给大家带来一篇干货。 Android的主题换肤 ，可插件化提供皮肤包，无需Activity的重启直接实现无缝切换,可高仿网易云音乐的主题换肤。

* [Android 主题动态切换框架：Prism](https://blog.leancloud.cn/3612/)

## 3.实现Android网络请求框架

* [打造属于自己的Android网络库](http://www.jianshu.com/p/16736df632a1)

	Android学习中网络是必不可少的一部分，甚至是重中之重。开发中可能我们会使用一些很成熟优秀的网络框架，如：OkHttp，Retrofit，Volley等。图片库：Fresco，Glide，Picasso，ImageLoader等。为了深入的学习一起来打造一个属于自己的网络库吧。
	
* [Android网络操作和优化相关](http://android.jobbole.com/83394/)

	Android程序最重要的模块就是网络部分，如何从网络上下载数据，如何将处理过的数据上传至网络，往往是android程序的关键环节。前几天偶一朋友遇到这么一个问题：如何使用volley实现文件上传。


## 4.实现Android图片加载框架

* [Google I/O 2013:Volley加载图片添加缓存处理](http://android.jobbole.com/81287/)

	Google I/O 2013已经结束，它让我们对Android将来的发展有了更大的期待。今年I/O大会上展示的令人激动的创新之一是名为Volley库。Volley是一个处理并缓存网络请求的库，它把开发者从不同的应用中编写相同代码的泥潭中拯救出来。编写相同代码从来都不是有趣的，还会增加开发者的错误几率。正式考虑了这一点，Google创造了Volley。
	
* [网络图片加载的封装【从零开始搭建android框架系列（4）】](http://www.jianshu.com/p/e26130a93289)


## 5.Android代码混淆

* [读懂 Android 中的代码混淆](http://droidyue.com/blog/2016/07/10/understanding-android-obfuscated-code-by-proguard/)

	介绍一些混淆的知识和注意事项
	
* [Android studio使用心得(五)---代码混淆和破解apk](http://my.oschina.net/aibenben/blog/371889)

* [ProGuard详解](http://seniorzhai.github.io/2016/04/11/ProGuard%E8%AF%A6%E8%A7%A3/)

* [Android进阶之ProGuard代码混淆](http://hanhailong.com/2015/12/28/Android%E8%BF%9B%E9%98%B6%E4%B9%8BProGuard%E4%BB%A3%E7%A0%81%E6%B7%B7%E6%B7%86/)

* [美团Android资源混淆保护实践](http://tech.meituan.com/mt-android-resource-obfuscation.html)

## 6.Android内测泄漏检测

* [用LeakCanary检测内存泄漏](https://realm.io/cn/news/droidcon-ricau-memory-leaks-leakcanary/)

	LeakCanary是一个帮助检测和修复内存泄漏的工具。

## 7.Realm

* [Realm快速入门](https://realm.io/cn/docs/java/latest/#section)

	更好的移动端数据库意味着更好的移动端应用。Realm 快速、易用并且免费，深受开发者和亿万用户喜爱。

## 8.RxJava和RxAndroid

* [Airbnb：我们的安卓客户端是如何使用 RxJava 的(Felipe Lima)](https://realm.io/cn/news/kau-felipe-lima-adopting-rxjava-airbnb-android/)

	Reactive编程和RxJava是最近常常引起强烈争论的话题，争论过程中问题很多，不确定性也很多。在Airbnb的客户端里，我们是如何采纳这些范式和技术，包括动力，实现的困难，和这一路走来的经验教训。我们还会看些产品的代码，比较 imperative编程和reactive编程的优劣，然后分别讨论它们的优势和缺陷。
	
* [带你学开源项目：RxLifecycle － 当Activity被destory时自动暂停网络请求](http://android.jobbole.com/83847/)

	本文分析思路不是从源码里抽代码出来一步步跟踪，而是提出问题，一步步思考解决方法，从而学习到开源项目的思维精华，而不仅仅是了解该项目的具体实现。笔者认为这种方式更有利于读者提高自身思维方式和技术能力。
    
* [RxAndroid+RxLifecycle+MVP实现异步请求，ButterKnife更新ui](http://www.infocool.net/kb/Android/201607/170013.html)

	各位好，今天的内容应该算是一个小框架了，使用Rx系列配合MVP实现异步请求，使用ButterKnife注入框架更新ui。 今天我主要讲的，今天的内容应该算是一个小框架了，使用Rx系列配合MVP实现异步请求，使用ButterKnife注入框架更新ui。今天我主要讲的是 RxAndroid+RxLifecycle+MVP+ButterKnife整体结合的小框架。


## 9.Android中的HTTPS

* [HTTPS 理论基础及其在 Android 中的最佳实践](http://android.jobbole.com/83787/)

	我们知道，HTTP请求都是明文传输的，所谓的明文指的是没有经过加密的信息，如果HTTP请求被黑客拦截，并且里面含有银行卡密码等敏感数据的话，会非常危险。为了解决这个问题，Netscape 公司制定了HTTPS协议，HTTPS可以将数据加密传输，也就是传输的是密文，即便黑客在传输过程中拦截到数据也无法破译，这就保证了网络通信的安全。
	

## 10.Android自定义view

* [Android自定义view详解](http://android.jobbole.com/83835/)

	对于我这样一个Android初级开发者来说，自定义View一直是一个遥不可及的东西，每次看到别人做的特别漂亮的控件，自己心里那个痒痒啊，可是又生性懒惰，自己不肯努力去看书，只能望而兴叹，每次做需求用到自定义控件，就直接去Github上找，找到合适的就用，找不到合适的，凑合也用，反正从来没想过要自己来做这样的东西，可是毕业以后到了新公司，为了自己的荣誉，这次不得不硬着头皮自己来了，一个月的紧张开发过后，回头再看，自定义控件也无非那么回事，只要记得几个要领，几乎是手到擒来。
	
## 11.Android事件分发

* [Android 中的事件分发和处理](http://android.jobbole.com/83826/)

	上次跟大家分享了一下自定义View的一下要点，这次跟大家聊一下View的事件分发及处理，为什么主题都是View，因为作为一名初级应用层Android工程师，跟我打交道最多的莫过于各种各样的View，只有详细了解他们各自的习性，才能更好地跟他们沟通交流，做出自己想要的效果。
	
## 12.Android插件化开发

* [Android插件化原理解析(1):概要](http://android.jobbole.com/82746/)

	2015年是Android插件化技术突飞猛进的一年，随着业务的发展各大厂商都碰到了Android Native平台的瓶颈：

	从技术上讲，业务逻辑的复杂导致代码量急剧膨胀，各大厂商陆续出到65535方法数的天花板；同时，运营为王的时代对于模块热更新提出了更高的要求。
	
	在业务层面上，功能模块的解耦以及维护团队的分离也是大势所趋；各个团队维护着同一个App的不同模块，如果每个模块升级新功能都需要对整个app进行升级，那么发布流程不仅复杂而且效率低下；在讲究小步快跑和持续迭代的移动互联网必将遭到淘汰。
	
* [Android插件化原理解析(2):Hook机制之动态代理](http://android.jobbole.com/83143/)

	使用代理机制进行API Hook进而达到方法增强是框架的常用手段，比如J2EE框架Spring通过动态代理优雅地实现了AOP编程，极大地提升了Web开发效率；同样，插件框架也广泛使用了代理机制来增强系统API从而达到插件化的目的。本文将带你了解基于动态代理的Hook机制。
	
* [Android插件化原理解析(3):Hook机制之Binder Hook](http://android.jobbole.com/83149/)

	Android系统通过Binder机制给应用程序提供了一系列的系统服务，诸如ActivityManagerService，ClipboardManager， AudioManager等；这些广泛存在系统服务给应用程序提供了诸如任务管理，音频，视频等异常强大的功能。

	插件框架作为各个插件的管理者，为了使得插件能够无缝地使用这些系统服务，自然会对这些系统服务做出一定的改造(Hook)，使得插件的开发和使用更加方便，从而大大降低插件的开发和维护成本。比如，Hook住ActivityManagerService可以让插件无缝地使用startActivity方法而不是使用特定的方式(比如that语法)来启动插件或者主程序的任意界面。
	
* [Android插件化原理解析(4):Hook机制之AMS&PMS](http://android.jobbole.com/83157/)

	在前面的文章中我们介绍了DroidPlugin的Hook机制，也就是代理方式和Binder Hook；插件框架通过AOP实现了插件使用和开发的透明性。在讲述DroidPlugin如何实现四大组件的插件化之前，有必要说明一下它对ActivityManagerServiche以及PackageManagerService的Hook方式（以下简称AMS，PMS）。
	
* [Android插件化原理解析(5):Activity生命周期管理](http://android.jobbole.com/83168/)

	之前的 Android插件化原理解析 系列文章揭开了Hook机制的神秘面纱，现在我们手握倚天屠龙，那么如何通过这种技术完成插件化方案呢？具体来说，插件中的Activity，Service等组件如何在Android系统上运行起来？
	
* [Android插件化原理解析(6):插件加载机制](http://android.jobbole.com/83175/)

	上文 Activity生命周期管理 中我们地完成了『启动没有在AndroidManifest.xml中显式声明的Activity』的任务；通过Hook AMS和拦截ActivityThread中H类对于组件调度我们成功地绕过了AndroidMAnifest.xml的限制。
	
* [Android插件化原理解析(7):广播的管理](http://android.jobbole.com/82776/)

	在Activity生命周期管理 以及 插件加载机制 中我们详细讲述了插件化过程中对于Activity组件的处理方式，为了实现Activity的插件化我们付出了相当多的努力；那么Android系统的其他组件，比如BroadcastReceiver，Service还有ContentProvider，它们又该如何处理呢？
	
* [Android插件化原理解析(8):ContentProvider的插件化](http://android.jobbole.com/83817/)

	目前为止我们已经完成了Android四大组件中Activity，Service以及BroadcastReceiver的插件化，这几个组件各不相同，我们根据它们的特点定制了不同的插件化方案；那么对于ContentProvider，它又有什么特点？应该如何实现它的插件化？
	

## 13.Android Dex分包

* [Android dex分包方案](http://android.jobbole.com/82328/)

	当一个app的功能越来越复杂，代码量越来越多，也许有一天便会突然遇到下列现象：

	(1)生成的apk在2.3以前的机器无法安装，提示INSTALL_FAILED_DEXOPT

	(2)方法数量过多，编译时出错，提示：

	Conversion to Dalvik format failed:Unable to execute dex: method ID not in [0, 0xffff]: 65536  

	出现这种问题的原因是：

	(1)Android2.3及以前版本用来执行dexopt(用于优化dex文件)的内存只分配了5M

	(2)一个dex文件最多只支持65536个方法。
	
* [美团Android DEX自动拆包及动态加载简介](http://android.jobbole.com/81218/)

	作为一个android开发者，在开发应用时，随着业务规模发展到一定程度，不断地加入新功能、添加新的类库，代码在急剧的膨胀，相应的apk包的大小也急剧增加， 那么终有一天，你会不幸遇到这个错误：

	(1)生成的apk在android 2.3或之前的机器上无法安装，提示INSTALL_FAILED_DEXOPT

	(2)方法数量过多，编译时出错，提示：
	
		Conversion to Dalvik format failed:Unable to execute dex: method ID not in [0, 0xffff]: 65536


## 14.Apk瘦身

* [Android APK瘦身实践](http://android.jobbole.com/82401/)

* [Android着色器Tint研究](http://android.jobbole.com/83875/)

	Tint 这个东西 主要用来减少apk体积的，比如说我现在有一个textview，他的背景图 有两种，一种是当获得焦点时显示的a图，另一种是 失去焦点时显示的b图。



## 15.Android线程池

* [Android 性能优化之使用线程池处理异步任务](http://android.jobbole.com/82092/#comment-91762)


## 16.RecyclerView优化

* [滑动时图片优化方案描述](http://www.2cto.com/kf/201509/443534.html)

	控制线程数量 + 数据分页加载

	我们在使用滑动控件呈现图片数据时，显然都会在getView方法里创建新的线程去异步加载图片，不可能有一百条或上千条数据一口气全部塞过来吧（当然你要这么干也是可以的），那么根据项目需求必然会进行分页加载，咱一页显示的item条数也别太夸张就好。而且，当我们点击屏幕快速向下滑动时，每个Item都会调用getView一次，必然会创建出很多线程去加载图片的URL资源，控制好线程的数量，加个线程池就非常有必要了。为了避免OOM导致FC，注意图片需要缓存，因为从内存中读取图片资源是非常快的。

	重写onScrollStateChanged方法

	这种方案用的也很普遍，相信只要细心观察，就会发现类似微博、Facebook、或者一些图片壁纸类的APP，在滑动时未加载的图片是不会立刻加载呈现的，只有当滑动停止后才会加载，这里需要注意一点的是，只加载当前屏幕内的图片。这么一说可能有童鞋就明白了。我们可以通过继承RecyclerView去自定义一个滑动控件，通过继承OnScrollListener后重写其 onScrolled方法 和 onScrollStateChanged 等方法来做相应处理。
	
* [值得收藏的 ViewHolder 工具类实现](http://android.jobbole.com/83917/)

	在开发APP的过程中，攻城狮少不了要跟ListView、GridView这些组件眉来眼去，暗送几波秋波。自然原生态美人BaseAdapter更是程序员的最爱，有了它，我们想怎么干就能怎么干，嘿嘿，你懂的O(∩_∩)O哈哈~

	但是，每次写一个BaseAdapter，我们都很自觉的给他写一个ViewHolder，一两个还好，万一应用程序中有数不清的ListView，呵呵~你妹！千篇一律，看得都审美疲劳。作为最伟大的第二十二世纪的程序员们，脱掉、搞上永远是我们最真挚的追求，所以我们要怎么将ViewHolder从BaseAdapter中脱掉呢？绝非不是不用，而是要将其搞成一个华丽丽的工具类实现，收入角落那个寂寞得tools类中。
	
## 17.Android性能优化

* [Android 性能优化之被忽视的内存泄漏](http://android.jobbole.com/83898/)

	写博客就像讲故事，得有起因，经过，结果，人物，地点和时间。今天就容我给大家讲一个故事。人物呢，肯定是我了。故事则发生在最近的这两天,地点在coder君上班的公司。那天无意中我发现了一个奇怪的现象，随着我点开我们App的页面，Memory Monitor中显示占用的内存越来越多（前面的页面已经finish掉了）。咦？什么鬼？
	
* [Android应用启动优化:一种DelayLoad的实现和原理(上篇)](http://android.jobbole.com/82366/)

* [Android应用启动优化:一种DelayLoad的实现和原理(下篇)](http://android.jobbole.com/82369/)

* [Android APP内存优化之图片优化](http://android.jobbole.com/83782/)

	网上有很多大拿分享的关于Android性能优化的文章，主要是通过各种工具分析，使用合理的技巧优化APP的体验，提升APP的流畅度，但关于内存优化的文章很少有看到。在Android设备内存动不动就上G的情况下，的确没有必要去太在意APP对Android系统内存的消耗，但在实际工作中我做的是教育类的小学APP，APP中的按钮、背景、动画变换基本上全是图片，在2K屏上（分辨率2048*1536）一张背景图片就会占用内存12M，来回切换几次内存占用就会增涨到上百兆，为了在不影响APP的视觉效果的前提下，有必要通过各种手段来降低APP对内存的消耗，下面是我在实践过程中使用的一些方法，很多都是不太成熟的项目，也不够深入，只是将其作为一种处理方式分享给大家。

	通过DDMS的APP内存占用查看工具分析发现，APP中占用内存最多的是图片，每个Activity中图片占用内存占大半，本文重点分享对图片的内存优化。
	
* [Android UI性能优化实战 识别绘制中的性能问题](http://android.jobbole.com/80947/)

	2015年初google发布了Android性能优化典范，发了16个小视频供大家欣赏，当时我也将其下载，通过微信公众号给大家推送了百度云的下载地址（地址在文末，ps:欢迎大家订阅公众号），那么近期google又在udacity上开了系列类的相关课程。有了上述的参考，那么本性能优化实战教程就有了坚实的基础，本系列将结合实例为大家展示如何去识别、诊断、解决Android应用开发中存在的性能问题。那么首先带来的就是大家最关注的渲染的性能优化（~~渲染就是把东西绘制到屏幕上）。

## 18.Android进程间通信

* [Android 手写 Binder 教你理解 android 中的进程间通信](http://android.jobbole.com/83957/)

	其实就从我们普通app开发者的角度来看，仅仅对于android应用层的话，Binder就是客户端和服务端进行通信的媒介。
	
* [Android 多进程编程 15问15答！](http://android.jobbole.com/83920/)

	阅读本文 需要对android 多进程编程有一定了解。
	

## 19.ListView相关

* [ListView中的RecycleBin机制](http://android.jobbole.com/83870/)

	此处会传入一个convertView变量，它的值有可能是null，也有可能不是null，如果不为null，我们就可以复用该convertView，对convertView里面的一些控件赋值后可以将convertView作为getView的返回值返回，这么做的目的是减少LayoutInflater.inflate()的调用次数，从而提升了性能（LayoutInflater.inflate()比较消耗性能）。

	本文将介绍ListView中的RecycleBin机制，让大家对ListView中的优化机制有个概括的了解，同时也说明convertView的来龙去脉。
	
* [Listview异步加载图片之优化篇](http://www.jcodecraeer.com/a/anzhuokaifa/androidkaifa/2013/0303/948.html)

	在 APP应用中，listview的异步加载图片方式能够带来很好的用户体验，同时也是考量程序性能的一个重要指标。关于listview的异步加载，网上 其实很多示例了，中心思想都差不多，不过很多版本或是有bug，或是有性能问题有待优化。有鉴于此，本人在网上找了个相对理想的版本并在此基础上进行改 造，下面就让在下阐述其原理以探索个中奥秘

	
## 20.从零开始的Android新项目系列

* [从零开始的Android新项目(1)：架构搭建篇](http://android.jobbole.com/82624/)
* [从零开始的Android新项目(2)：Gradle篇](http://android.jobbole.com/82747/)
* [从零开始的Android新项目(3)：谁告诉你MVP和MVVM是互斥的](http://android.jobbole.com/82809/)
* [从零开始的Android新项目(4)：Dagger2篇](http://android.jobbole.com/82820/)
* [从零开始的Android新项目(5)：Repository层(上)](http://android.jobbole.com/83210/)
* [从零开始的Android新项目(6)：Repository层(下)](http://android.jobbole.com/83234/)
* [从零开始的Android新项目(7)：Data Binding入门篇](http://android.jobbole.com/83688/)
* [从零开始的Android新项目(8)：Data Binding高级篇](http://android.jobbole.com/83842/)

## 21.Handler相关

* [Android消息处理机制：Handler|Message](http://android.jobbole.com/83823/)

	在日常开发中，不管出于什么目的，我们可能都会用到Handler来异步更新UI，有时是为了将一些费时的操作放到异步线程去处理，然后通过Handler将数据更新到UI线程，有时是为了在子线程里更新UI，种种原因，反正我们最后都是选择了直接的Handler+Message组合或者AsyncTask，而了解AsyncTask的同学都知道，AsyncTask内部就是通过Handler和Message实现的线程间通信，所以我们还是要好好熟悉一下这位老朋友
	
	
## 22.Android资源动态加载

* [Android apk动态加载机制的研究](http://www.jcodecraeer.com/a/anzhuokaifa/androidkaifa/2014/1013/1759.html)

	首先宿主程序会到文件系统比如sd卡去加载apk，然后通过一个叫做proxy的activity去执行apk中的activity。
关于动态加载apk，理论上可以用到的有DexClassLoader、PathClassLoader和URLClassLoader。
DexClassLoader ：可以加载文件系统上的jar、dex、apk.

## 23.Android与js沟通

* [好好和h5沟通！几种常见的hybrid通信方式](http://www.jcodecraeer.com/a/anzhuokaifa/androidkaifa/2016/0418/4157.html)

	说起hybrid大家不会陌生，主要意思就是native和h5混合开发。为什么要这样做呢？大家可以想象一下针对于同一个活动，如果使用纯native的开发方式，Android和iOS两边都要维护同一套界面甚至是逻辑，这样开发和维护的成本会很大，而使用hybrid的开发方式的话，让前端的同学去写一套界面和逻辑，对于native端来说只要使用对应的容器去展示就可以了(对于Android来说这个容器当然就是WebView)。那为什么不所有的页面都使用这种方式开发呢？因为使用h5来展示界面的话用户体验始终是不如native的，所以在这两者之间我们需要一个权衡。
	
	
## 24.Android apk动态加载机制的研究

* [Android apk动态加载机制的研究(一)](http://www.jcodecraeer.com/a/anzhuokaifa/androidkaifa/2014/1013/1759.html)

* [Android apk动态加载机制的研究(二):资源加载和activity生命周期管理](http://www.jcodecraeer.com/a/anzhuokaifa/androidkaifa/2014/1013/1760.html)

## 25.Android多进程

* [Android多进程编程15问15答](http://android.jobbole.com/83920/)

	阅读本文 需要对android 多进程编程有一定了解
	
* [Android应用内多进程的使用及注意事项](http://android.jobbole.com/83771/)

	一个应用默认只有一个进程，这个进程（主进程）的名称就是应用的包名，进程是系统分配资源和调度的基本单位，每个进程都有自己独立的资源和内存空间，其它进程不能任意访问当前进程的内存和资源，系统给每个进程分配的内存会有限制。
	
* [关于Android进程保活，你所需要知道的一切](http://android.jobbole.com/82815/)

	关于 Android 平台的进程保活这一块，想必是所有 Android 开发者瞩目的内容之一。你到网上搜 Android 进程保活，可以搜出各种各样神乎其技的做法，绝大多数都是极其不靠谱。前段时间，Github还出现了一个很火的“黑科技”进程保活库，声称可以做到进程永生不死。

	

## 26.Android系统级原理

* [理解Android安全机制](http://android.jobbole.com/82409/)

	本文从Android系统架构着手，分析Android的安全机制以SE Android，最后给出一些Android安全现状和常见的安全解决方案。
	

## 27.RxJava+Retrofit+Dagger2

* [带你学开源项目：Meizhi Android之RxJava&Retrofit最佳实践](http://android.jobbole.com/82737/)


## 28.Android优化工具

* [值得推荐的Android应用性能检测工具列表](http://android.jobbole.com/82572/)


## 29.Android新编译系统

* [Android 应用开发编译框架流程与IDE及Gradle概要](http://android.jobbole.com/82031/)

## 30.Android注解框架

* [Android 打造编译时注解解析框架 这只是一个开始](http://android.jobbole.com/80977/)

## 31.Material Design相关

* [Material Design 开发利器：Android Design Support Library 介绍](https://blog.leancloud.cn/3306/)

## 32 butterknife相关

* [butterknife官网](http://jakewharton.github.io/butterknife/)

## 33 MVP架构

* [一步一步实现Android的MVP框架](http://mp.weixin.qq.com/s?__biz=MzA3NTYzODYzMg%3D%3D&idx=1&mid=2653577546&scene=1&sn=e10be159645a3aa8f6d6f209420fb412&srcid=07289Nbf5unjDpiRXxvw1G90)

	1.Android 开发框架的选择

	2.如何一步步搭建分层框架
	
    3.使用 RxJava 来解决主线程发出网络请求的问题

* [浅谈Andorid开发中的MVP模式](http://www.jcodecraeer.com/a/anzhuokaifa/androidkaifa/2016/0225/3994.html)

	看到MVP，大家肯定会想什么是MVP呢？这个我可以肯定的告诉大家MVP（Most Valuable Player）是最有价值球员的意思，这当然是开玩笑了。之所以会出现MVP这种架构模式，是因为我相信大家在开发App时，肯定会发现，Activity的负担非常重，既要初始化控件，又要写一些逻辑操作的展示等等，有时候很多Activity中的代码都充当了Controller和Model的角色，所以你会发现Activity违背单一职责原则，负担过重。所以，就出现了这么一种架构模式，叫MVP，并不是最有价值球员哦。
	
	
* 测试Github是否可用

## 34 Gradle相关

- [加速Android Studio/Gradle构建](http://blog.isming.me/2015/03/18/android-build-speed-up/)

效果很明显啊！之前的构建时间为20分钟，添加了配置之后构建时间仅为36秒！！！

- [Android模块化编程之引用本地的aar](http://stormzhang.com/android/2015/03/01/android-reference-local-aar/)

jar：java代码

aar：包含java代码和资源文件

- [mvn-repo](https://github.com/Goddchen/mvn-repo)

- [常用的Gradle命令](http://seniorzhai.github.io/2015/08/16/%E5%B8%B8%E7%94%A8%E7%9A%84Gradle%E5%91%BD%E4%BB%A4/)


- [Android Studio通过Gradle命令来编译生成打包APK(Windows版本)](http://www.whatjay.com/?p=999)

- [android studio生成aar包并在其他工程引用aar包](http://www.mobile-open.com/2016/972218.html)

## 35 进行保活

- [Android 进程保活招式大全](https://mp.weixin.qq.com/s?__biz=MzA3NTYzODYzMg==&mid=2653577617&idx=1&sn=623256a2ff94641036a6c9eea17baab8)







