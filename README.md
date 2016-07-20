# Android进阶技能点


## RecyclerView


* [深入浅出RecyclerView(张涛)](http://kymjs.com/code/2016/07/10/01)

	介绍RecyclerView的基本用法、原理分析及其源码解析。

* [RecyclerView的通用适配器，和滚动时不加载图片的封装(张涛)](http://kymjs.com/code/2015/10/11/01)

	介绍RecyclerView的BaseAdapter、BaseViewHolder的封装，及滑动图片不加载。


## Android主题切换

* [Android夜间模式实现](http://kymjs.com/code/2015/05/26/01)

	介绍实现主题切换的简单实现思路，通过一个Demo进行讲解。

* [Android主题换肤的开源库ThemeSkinning](http://android.jobbole.com/83662/)

	本开源库是基于我之前的一个博客 Android主题换肤 无缝切换 不知道原理的可以去这篇博客看看。出于易于集成的目的，我将其抽取出来，作为一个模块。提供简洁的api，方便使用。
	
* [Android主题换肤无缝切换](http://android.jobbole.com/82932/)

	今天再给大家带来一篇干货。 Android的主题换肤 ，可插件化提供皮肤包，无需Activity的重启直接实现无缝切换,可高仿网易云音乐的主题换肤。
	



## 实现Android网络请求框架

* 

## 实现Android图片加载框架



## Android代码混淆

* [读懂 Android 中的代码混淆](http://droidyue.com/blog/2016/07/10/understanding-android-obfuscated-code-by-proguard/)

	介绍一些混淆的知识和注意事项

## Android内测泄漏检测

* [用LeakCanary检测内存泄漏](https://realm.io/cn/news/droidcon-ricau-memory-leaks-leakcanary/)

	LeakCanary是一个帮助检测和修复内存泄漏的工具。

## Realm

* [Realm快速入门](https://realm.io/cn/docs/java/latest/#section)

	更好的移动端数据库意味着更好的移动端应用。Realm 快速、易用并且免费，深受开发者和亿万用户喜爱。

## RxJava和RxAndroid

* [Airbnb：我们的安卓客户端是如何使用 RxJava 的(Felipe Lima)](https://realm.io/cn/news/kau-felipe-lima-adopting-rxjava-airbnb-android/)

	Reactive编程和RxJava是最近常常引起强烈争论的话题，争论过程中问题很多，不确定性也很多。在Airbnb的客户端里，我们是如何采纳这些范式和技术，包括动力，实现的困难，和这一路走来的经验教训。我们还会看些产品的代码，比较 imperative编程和reactive编程的优劣，然后分别讨论它们的优势和缺陷。

## Android中的HTTPS

* [HTTPS 理论基础及其在 Android 中的最佳实践](http://android.jobbole.com/83787/)

	我们知道，HTTP请求都是明文传输的，所谓的明文指的是没有经过加密的信息，如果HTTP请求被黑客拦截，并且里面含有银行卡密码等敏感数据的话，会非常危险。为了解决这个问题，Netscape 公司制定了HTTPS协议，HTTPS可以将数据加密传输，也就是传输的是密文，即便黑客在传输过程中拦截到数据也无法破译，这就保证了网络通信的安全。
	

## Android自定义view

* [Android自定义view详解](http://android.jobbole.com/83835/)

	对于我这样一个Android初级开发者来说，自定义View一直是一个遥不可及的东西，每次看到别人做的特别漂亮的控件，自己心里那个痒痒啊，可是又生性懒惰，自己不肯努力去看书，只能望而兴叹，每次做需求用到自定义控件，就直接去Github上找，找到合适的就用，找不到合适的，凑合也用，反正从来没想过要自己来做这样的东西，可是毕业以后到了新公司，为了自己的荣誉，这次不得不硬着头皮自己来了，一个月的紧张开发过后，回头再看，自定义控件也无非那么回事，只要记得几个要领，几乎是手到擒来。
	
## Android事件分发

* [Android 中的事件分发和处理](http://android.jobbole.com/83826/)

	上次跟大家分享了一下自定义View的一下要点，这次跟大家聊一下View的事件分发及处理，为什么主题都是View，因为作为一名初级应用层Android工程师，跟我打交道最多的莫过于各种各样的View，只有详细了解他们各自的习性，才能更好地跟他们沟通交流，做出自己想要的效果。
	
## Android插件化开发

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
	

## Android Dex分包

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


## Apk瘦身

* [Android APK瘦身实践](http://android.jobbole.com/82401/)

## Android线程池

* [Android 性能优化之使用线程池处理异步任务](http://android.jobbole.com/82092/#comment-91762)


## RecyclerView优化

* [滑动时图片优化方案描述](http://www.2cto.com/kf/201509/443534.html)

	控制线程数量 + 数据分页加载

	我们在使用滑动控件呈现图片数据时，显然都会在getView方法里创建新的线程去异步加载图片，不可能有一百条或上千条数据一口气全部塞过来吧（当然你要这么干也是可以的），那么根据项目需求必然会进行分页加载，咱一页显示的item条数也别太夸张就好。而且，当我们点击屏幕快速向下滑动时，每个Item都会调用getView一次，必然会创建出很多线程去加载图片的URL资源，控制好线程的数量，加个线程池就非常有必要了。为了避免OOM导致FC，注意图片需要缓存，因为从内存中读取图片资源是非常快的。

	重写onScrollStateChanged方法

	这种方案用的也很普遍，相信只要细心观察，就会发现类似微博、Facebook、或者一些图片壁纸类的APP，在滑动时未加载的图片是不会立刻加载呈现的，只有当滑动停止后才会加载，这里需要注意一点的是，只加载当前屏幕内的图片。这么一说可能有童鞋就明白了。我们可以通过继承RecyclerView去自定义一个滑动控件，通过继承OnScrollListener后重写其 onScrolled方法 和 onScrollStateChanged 等方法来做相应处理。
	


















	












