AndroidManiFest总目录


[TOC]



## manifest

### 语法

```xml
<manifest xmlns:android="http://schemas.android.com/apk/res/android"//定义命名空间，必须
          package="string"//包名
          android:sharedUserId="string"//将被分享给其他应用的linux用户id
          android:sharedUserLabel="string resource"//提供一个可读的标志为用户id
          android:versionCode="integer"//版本号
          android:versionName="string"//版本名称
          android:installLocation=["auto" | "internalOnly" | "preferExternal"]//默认安装目录
          >
    . . .
</manifest>
```

> 说明
1、internalOnly：应用必须安装在设备内部存储器。如果设置了这个属性，应用将不会被安装到外部设备。如果内部设备已经满了，系统将不会安装应用。如果不声明android:installLocation属性系统将会把安装到内部存储器作为默认选项。
2、auto：应用也许会被安装到外部存储器上，但是默认情况下，应用会被系统安装到内部存储器。如果内部存储器已经满了，系统将会把应用安装到外部存储器。一旦安装成功，用户可以通过设置选项将应用的安装目录在内部存储器与外部存储器之间切换。
3、preferExternal：应用更喜欢被安装到外部存储器（即SD卡）。这儿不能保证系统将处理这个请求。如果外部存储器不可用或已满，应用将会被安装到内部存储器。一旦安装，用户可以通过系统设置将应用安装位置在内部存储器与外部存储器之间切换。

[App Install Location](https://developer.android.com/guide/topics/data/install-location.html)

### 在以下标签中使用

无

### 必选属性

- application

### 可选属性

- compatible-screens
- instrumentation
- permission
- permission-group
- permission-tree
- supports-gl-texture
- supports-screens
- uses-configuration
- uses-feature
- uses-permission
- uses-permission-sdk-23
- uses-sdk

## intent-filter

### 语法

```xml
<intent-filter
 			android:icon="drawable resource"//一个icon代表父Activity、service、BroadcastReceiver 当那个组件出现在 用户通过filter描述容量之中
            android:label="string resource"//为父组件提供的一个可读的标志
            android:priority="integer">//赋予父组件的优先级关于操作被filter描述的intent类型
    <action android:name="android.intent.action.MAIN" />//为intent filter添加Action
    <data android:host="@string/app_name"/>//为intent filter添加data说明
    <category android:name="android.intent.category.LAUNCHER" />//为intent filter添加一个category名称
</intent-filter>
```

### 在以下标签中使用

- activity
- activity-alias
- service
- receiver

### 必须包含属性

- action

### 可选属性

- category
- data

## activity-alias

### 语法

```xml
<activity-alias android:enabled=["true" | "false"]//目标Activity是否可以通过别名被系统实例化
                android:exported=["true" | "false"]//其他应用是否可以加载目标Activity通过这个别名
                android:icon="drawable resource"//通过别名目标Activity呈现给用户的icon
                android:label="string resource"//通过别名目标Activity呈现给用户的标志
                android:name="string"//一个为别名的唯一标志
                android:permission="string"//客户端加载目标Activity或通过别名做一些事情需要的权限名称
                android:targetActivity="string" >//通过别名可以被激活的Activity的名称
    . . .
</activity-alias>
```

### 在以下标签中包含

- application

### 可选属性

- intent-filter
- meta-data

## application

### 语法

```xml
<application android:allowTaskReparenting=["true" | "false"]
             android:allowBackup=["true" | "false"]
             android:backupAgent="string"
             android:banner="drawable resource"
             android:debuggable=["true" | "false"]
             android:description="string resource"
             android:enabled=["true" | "false"]
             android:hasCode=["true" | "false"]
             android:hardwareAccelerated=["true" | "false"]
             android:icon="drawable resource"
             android:isGame=["true" | "false"]
             android:killAfterRestore=["true" | "false"]
             android:largeHeap=["true" | "false"]
             android:label="string resource"
             android:logo="drawable resource"
             android:manageSpaceActivity="string"
             android:name="string"
             android:permission="string"
             android:persistent=["true" | "false"]
             android:process="string"
             android:restoreAnyVersion=["true" | "false"]
             android:requiredAccountType="string"
             android:resizeableActivity=["true" | "false"]
             android:restrictedAccountType="string"
             android:supportsRtl=["true" | "false"]
             android:taskAffinity="string"
             android:testOnly=["true" | "false"]
             android:theme="resource or theme"
             android:uiOptions=["none" | "splitActionBarWhenNarrow"]
             android:usesCleartextTraffic=["true" | "false"]
             android:vmSafeMode=["true" | "false"] >
    . . .
</application>
```

### 在以下标签中使用

- manifest

### 可选属性

- activity
- activity-alias
- meta-data
- service
- receiver
- provider
- uses-library

## activity

### 语法

```xml
<activity android:allowEmbedded=["true" | "false"]
          android:allowTaskReparenting=["true" | "false"]//是否允许activity更换从属的任务，比如从短信息任务切换到浏览器任务
          android:alwaysRetainTaskState=["true" | "false"]//是否保留状态不变， 比如切换回home, 再从新打开， activity处于最后的状态
          android:autoRemoveFromRecents=["true" | "false"]
          android:banner="drawable resource"
          android:clearTaskOnLaunch=["true" | "false"]//比如 P 是 activity, Q 是被P 触发的 activity, 然后返回Home, 从新启动 P，是否显示 Q
          android:configChanges=["mcc", "mnc", "locale",
                                 "touchscreen", "keyboard", "keyboardHidden",
                                 "navigation", "screenLayout", "fontScale",
                                 "uiMode", "orientation", "screenSize",
                                 "smallestScreenSize"]
                                 //当配置list发生修改时，是否调用 onConfigurationChanged() 方法 比如 “locale|navigation|orientation”
          android:documentLaunchMode=["intoExisting" | "always" |
                                  "none" | "never"]
          android:enabled=["true" | "false"]//activity 是否可以被实例化
          android:excludeFromRecents=["true" | "false"]//是否可被显示在最近打开的activity列表里
          android:exported=["true" | "false"]//是否允许activity被其它程序调用
          android:finishOnTaskLaunch=["true" | "false"]//是否关闭已打开的activity当用户重新启动这个任务的时候
          android:hardwareAccelerated=["true" | "false"]
          android:icon="drawable resource"
          android:label="string resource"
          android:launchMode=["standard" | "singleTop" |
                              "singleTask" | "singleInstance"]//activity启动方式， “standard” “singleTop” “singleTask” “singleInstance”
其中前两个为一组， 后两个为一组
          android:maxRecents="integer"
          android:multiprocess=["true" | "false"]//允许多进程
          android:name="string"
          android:noHistory=["true" | "false"]//是否需要移除这个activity当用户切换到其他屏幕时
          android:parentActivityName="string" 
          android:permission="string"
          android:process="string"//一 个activity运行时所在的进程名，所有程序组件运行在应用程序默认的进程中，这个进程名跟应用程序的包名一致。中的元素process属性能够为所有组件设定一个新的默认值。但是任何组件都可以覆盖这个默认值，允许你将你的程序放在多进程中运行。 如果这个属性被分配的名字以:开头，当这个activity运行时, 一个新的专属于这个程序的进程将会被创建。如果这个进程名以小写字母开头，这个activity将会运行在全局的进程中，被它的许可所提供。
          android:relinquishTaskIdentity=["true" | "false"]
          android:resizeableActivity=["true" | "false"]
          android:screenOrientation=["unspecified" | "behind" |
                                     "landscape" | "portrait" |
                                     "reverseLandscape" | "reversePortrait" |
                                     "sensorLandscape" | "sensorPortrait" |
                                     "userLandscape" | "userPortrait" |
                                     "sensor" | "fullSensor" | "nosensor" |
                                     "user" | "fullUser" | "locked"]//activity显示的模式, “unspecified” 默认值 “landscape” 风景画模式，宽度比高度大一些 “portrait” 肖像模式, 高度比宽度大。 “user” 用户的设置 “behind” “sensor” “nosensor”
          android:stateNotNeeded=["true" | "false"]//是否 activity被销毁和成功重启并不保存状态
          android:supportsPictureInPicture=["true" | "false"]
          android:taskAffinity="string"//activity的亲属关系， 默认情况同一个应用程序下的activity有相同的关系
          android:theme="resource or theme"
          android:uiOptions=["none" | "splitActionBarWhenNarrow"]
          android:windowSoftInputMode=["stateUnspecified",
                                       "stateUnchanged", "stateHidden",
                                       "stateAlwaysHidden", "stateVisible",
                                       "stateAlwaysVisible", "adjustUnspecified",
                                       "adjustResize", "adjustPan"] >//
    . . .
</activity>
```

**说明**：

- **stateUnspecified**	软键盘的状态(是否它是隐藏或可见)没有被指定。系统将选择一个合适的状态或依赖于主题的设置。这个是为了软件盘行为默认的设置。
- **stateUnchanged**	软键盘被保持无论它上次是什么状态，是否可见或隐藏，当主窗口出现在前面时。
- **stateHidden**	当用户选择该Activity时，软键盘被隐藏——也就是，当用户确定导航到该Activity时，而不是返回到它由于离开另一个Activity。
- **stateAlwaysHidden**	软键盘总是被隐藏的，当该Activity主窗口获取焦点时。
- **stateVisible**	软键盘是可见的，当那个是正常合适的时(当用户导航到Activity主窗口时)。
- **stateAlwaysVisible**	当用户选择这个Activity时，软键盘是可见的——也就是，也就是，当用户确定导航到该Activity时，而不是返回到它由于离开另一个Activity。
- **adjustUnspecified**	它不被指定是否该Activity主窗口调整大小以便留出软键盘的空间，或是否窗口上的内容得到屏幕上当前的焦点是可见的。系统将自动选择这些模式中一种主要依赖于是否窗口的内容有任何布局视图能够滚动他们的内容。如果有这样的一个视图，这个窗口将调整大小，这样的假设可以使滚动窗口的内容在一个较小的区域中可见的。这个是主窗口默认的行为设置。
- **adjustResize**	该Activity主窗口总是被调整屏幕的大小以便留出软键盘的空间。
- **adjustPan**	该Activity主窗口并不调整屏幕的大小以便留出软键盘的空间。相反，当前窗口的内容将自动移动以便当前焦点从不被键盘覆盖和用户能总是看到输入内容的部分。这个通常是不期望比调整大小，因为用户可能关闭软键盘以便获得与被覆盖内容的交互操作。



### 在以下标签中使用

- application

### 可选属性

- intent-filter
- meta-data

## meta-data

### 语法

```xml
<meta-data android:name="string"
           android:resource="resource specification"
           android:value="string" />
```

### 在以下标签中使用

- activity
- activity-alias
- application
- provider
- receiver

### 不可使用标签

- service

## service

### 语法

```xml
<service android:enabled=["true" | "false"]
         android:exported=["true" | "false"]
         android:icon="drawable resource"
         android:isolatedProcess=["true" | "false"]
         android:label="string resource"
         android:name="string"
         android:permission="string"
         android:process="string" >
    . . .
</service>
```

### 在以下标签中使用

- application

### 可选属性

- intent-filter
- meta-data

## receiver

### 语法

```xml
<receiver android:enabled=["true" | "false"]
          android:exported=["true" | "false"]
          android:icon="drawable resource"
          android:label="string resource"
          android:name="string"
          android:permission="string"
          android:process="string" >
    . . .
</receiver>
```

### 在以下标签中使用

- application

### 可选属性

- intent-filter
- meta-data

## provider

### 语法

```xml
<provider android:authorities="list"
          android:enabled=["true" | "false"]
          android:exported=["true" | "false"]
          android:grantUriPermissions=["true" | "false"]
          android:icon="drawable resource"
          android:initOrder="integer"
          android:label="string resource"
          android:multiprocess=["true" | "false"]
          android:name="string"
          android:permission="string"
          android:process="string"
          android:readPermission="string"
          android:syncable=["true" | "false"]
          android:writePermission="string" >
    . . .
</provider>
```

### 在以下标签中使用

- application

### 可选属性

- meta-data
- grant-uri-permission
- path-permission

## action

### 语法

```xml
<action android:name="string" />
```

### 在以下标签中使用

- intent-filter

## category

### 语法

```xml
<category android:name="string" />
```
### 在以下标签中使用

- intent-filter

## compatible-screens

### 语法

```xml
<compatible-screens>
    <screen android:screenSize=["small" | "normal" | "large" | "xlarge"]
            android:screenDensity=["ldpi" | "mdpi" | "hdpi" | "xhdpi"
                                   | "280" | "360" | "420" | "480" | "560" ] />
    ...
</compatible-screens>
```

### 在以下标签中使用

- manifest

## data

### 语法

```xml
<data android:scheme="string"
      android:host="string"
      android:port="string"
      android:path="string"
      android:pathPattern="string"
      android:pathPrefix="string"
      android:mimeType="string" />
```

### 在以下标签中使用

- intent-filter

## grant-uri-permission

### 语法

```xml
<grant-uri-permission android:path="string"
                      android:pathPattern="string"
                      android:pathPrefix="string" />
```

### 在以下标签中使用

- provider

## instrumentation

### 语法

```xml
<instrumentation android:functionalTest=["true" | "false"]
                 android:handleProfiling=["true" | "false"]
                 android:icon="drawable resource"
                 android:label="string resource"
                 android:name="string"
                 android:targetPackage="string" />
```

### 在以下标签中使用

- manifest

## path-permission

### 语法

```xml
<path-permission android:path="string"
                 android:pathPrefix="string"
                 android:pathPattern="string"
                 android:permission="string"
                 android:readPermission="string"
                 android:writePermission="string" />
```

### 在以下标签中使用

- provider

## permission

### 语法

```xml
<permission android:description="string resource"
            android:icon="drawable resource"
            android:label="string resource"
            android:name="string"
            android:permissionGroup="string"
            android:protectionLevel=["normal" | "dangerous" |
                                     "signature" | "signatureOrSystem"] />
```

### 在以下标签中使用

- manifest

## permission-group

### 语法

```xml
<permission-group android:description="string resource"
                  android:icon="drawable resource"
                  android:label="string resource"
                  android:name="string" />
```

### 在以下标签中使用

- manifest

## permission-tree

### 语法

```xml
<permission-tree android:icon="drawable resource"
                 android:label="string resource" ]
                 android:name="string" />
```

### 在以下标签中使用

- manifest

## supports-gl-texture

### 语法

```xml
<supports-gl-texture
  android:name="string" />
```

### 在以下标签中使用

- manifest

## supports-screens

### 语法

```xml
<supports-screens android:resizeable=["true"| "false"]
                  android:smallScreens=["true" | "false"]
                  android:normalScreens=["true" | "false"]
                  android:largeScreens=["true" | "false"]
                  android:xlargeScreens=["true" | "false"]
                  android:anyDensity=["true" | "false"]
                  android:requiresSmallestWidthDp="integer"
                  android:compatibleWidthLimitDp="integer"
                  android:largestWidthLimitDp="integer"/>
```

### 在以下标签中使用

- manifest

## uses-configuration

### 语法

```xml
<uses-configuration
  android:reqFiveWayNav=["true" | "false"]
  android:reqHardKeyboard=["true" | "false"]
  android:reqKeyboardType=["undefined" | "nokeys" | "qwerty" | "twelvekey"]
  android:reqNavigation=["undefined" | "nonav" | "dpad" | "trackball" | "wheel"]
  android:reqTouchScreen=["undefined" | "notouch" | "stylus" | "finger"] />
```

### 在以下标签中使用

- manifest

## uses-feature

### 语法

```xml
<uses-feature
  android:name="string"
  android:required=["true" | "false"]
  android:glEsVersion="integer" />
```

### 在以下标签中使用

- manifest

## uses-library

### 语法

```xml
<uses-library
  android:name="string"
  android:required=["true" | "false"] />
```

### 在以下标签中使用

- application

## uses-permission

### 语法

```xml
<uses-permission android:name="string"
        android:maxSdkVersion="integer" />
```

### 在以下标签中使用

- manifest

## uses-permission-sdk-23

### 语法

```xml
<uses-permission-sdk-23 android:name="string"
        android:maxSdkVersion="integer" />
```

### 在以下标签中使用

- manifest

## uses-sdk

### 语法

```xml
<uses-sdk android:minSdkVersion="integer"
          android:targetSdkVersion="integer"
          android:maxSdkVersion="integer" />
```

### 在以下标签中使用

- manifest




