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
          android:allowTaskReparenting=["true" | "false"]
          android:alwaysRetainTaskState=["true" | "false"]
          android:autoRemoveFromRecents=["true" | "false"]
          android:banner="drawable resource"
          android:clearTaskOnLaunch=["true" | "false"]
          android:configChanges=["mcc", "mnc", "locale",
                                 "touchscreen", "keyboard", "keyboardHidden",
                                 "navigation", "screenLayout", "fontScale",
                                 "uiMode", "orientation", "screenSize",
                                 "smallestScreenSize"]
          android:documentLaunchMode=["intoExisting" | "always" |
                                  "none" | "never"]
          android:enabled=["true" | "false"]
          android:excludeFromRecents=["true" | "false"]
          android:exported=["true" | "false"]
          android:finishOnTaskLaunch=["true" | "false"]
          android:hardwareAccelerated=["true" | "false"]
          android:icon="drawable resource"
          android:label="string resource"
          android:launchMode=["standard" | "singleTop" |
                              "singleTask" | "singleInstance"]
          android:maxRecents="integer"
          android:multiprocess=["true" | "false"]
          android:name="string"
          android:noHistory=["true" | "false"]  
          android:parentActivityName="string" 
          android:permission="string"
          android:process="string"
          android:relinquishTaskIdentity=["true" | "false"]
          android:resizeableActivity=["true" | "false"]
          android:screenOrientation=["unspecified" | "behind" |
                                     "landscape" | "portrait" |
                                     "reverseLandscape" | "reversePortrait" |
                                     "sensorLandscape" | "sensorPortrait" |
                                     "userLandscape" | "userPortrait" |
                                     "sensor" | "fullSensor" | "nosensor" |
                                     "user" | "fullUser" | "locked"]
          android:stateNotNeeded=["true" | "false"]
          android:supportsPictureInPicture=["true" | "false"]
          android:taskAffinity="string"
          android:theme="resource or theme"
          android:uiOptions=["none" | "splitActionBarWhenNarrow"]
          android:windowSoftInputMode=["stateUnspecified",
                                       "stateUnchanged", "stateHidden",
                                       "stateAlwaysHidden", "stateVisible",
                                       "stateAlwaysVisible", "adjustUnspecified",
                                       "adjustResize", "adjustPan"] >   
    . . .
</activity>
```

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




