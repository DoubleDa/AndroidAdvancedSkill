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