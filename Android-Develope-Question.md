# Android开发中的问题


[TOC]



## 使用ButterKnife的正确姿势

1、在项目的**build.gradle**中添加**android-apt**插件
```gradle
buildscript {
  repositories {
    mavenCentral()
   }
  dependencies {
    classpath 'com.neenbedankt.gradle.plugins:android-apt:1.8'
  }
}
```

2、在**app/build.gradle**中添加如下代码
```gradle
apply plugin: 'android-apt'

android {
  ...
}

dependencies {
  compile 'com.jakewharton:butterknife:8.4.0'
  apt 'com.jakewharton:butterknife-compiler:8.4.0'
}
```

## Java关键字native

[Java中的native关键字浅析（Java Native Interface）](http://blog.csdn.net/yangjiali014/article/details/1633017)



## Android序列化方式：Serializable和Parcelable


## [Android动态加载基础 ClassLoader工作机制](https://segmentfault.com/a/1190000004062880)

## [OkHttp跟Retrofit的区别](http://blog.csdn.net/lmj623565791/article/details/51304204)

## [自定义View](http://www.jianshu.com/p/d507e3514b65)

- View是怎样被显示到屏幕上的？

![](http://ob35pbpax.bkt.clouddn.com/%E8%87%AA%E5%AE%9A%E4%B9%89View.png?e=1473221466&token=b_hRB7WBnNMHUhLIZNEP-DlJC_-17UnRgWlnj5VG:v6s4lAQyjZ_BA32ceoSIYfr5DOU)

- 自定义View大小

![](http://ob35pbpax.bkt.clouddn.com/%E8%87%AA%E5%AE%9A%E4%B9%89View%E5%A4%A7%E5%B0%8F.png?e=1473222942&token=b_hRB7WBnNMHUhLIZNEP-DlJC_-17UnRgWlnj5VG:jPbWt2s671GHVrDmUJsM616GlSc)

- View的生命周期

![](http://ob35pbpax.bkt.clouddn.com/View%E7%9A%84%E7%94%9F%E5%91%BD%E5%91%A8%E6%9C%9F.png?e=1473229654&token=b_hRB7WBnNMHUhLIZNEP-DlJC_-17UnRgWlnj5VG:TMBPIR2_UXtK8HRRWZQNlYfFMyc)

- [View相关](https://developer.android.com/reference/android/view/View.html)



## JsBridge相关

[Android JSBridge的原理与实现](http://blog.csdn.net/sbsujjbcy/article/details/50752595)

## Hybrid开发

- [Hybrid APP架构设计思路](https://segmentfault.com/a/1190000004263182)

- [【腾讯bugly干货分享】解耦---Hybrid H5跨平台性思考](https://segmentfault.com/a/1190000005871087)


