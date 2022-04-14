## Crash Details

**Crash Thread**: `Thread[main,5,main]`  
**Crash Timestamp**: `2022-04-14 07:49:58.120 UTC`  

**Crash Message**:
```
Unable to start activity ComponentInfo{com.termux/com.termux.app.TermuxActivity}: java.lang.IllegalStateException: Not allowed to start service Intent { cmp=com.termux/.app.TermuxService }: app is in background uid UidRecord{3fb2066 u0a329 TPSL idle procs:1 seq(0,0,0)}
```


### Stacktrace

```
java.lang.RuntimeException: Unable to start activity ComponentInfo{com.termux/com.termux.app.TermuxActivity}: java.lang.IllegalStateException: Not allowed to start service Intent { cmp=com.termux/.app.TermuxService }: app is in background uid UidRecord{3fb2066 u0a329 TPSL idle procs:1 seq(0,0,0)}
	at android.app.ActivityThread.performLaunchActivity(ActivityThread.java:3634)
	at android.app.ActivityThread.handleLaunchActivity(ActivityThread.java:3879)
	at android.app.servertransaction.LaunchActivityItem.execute(LaunchActivityItem.java:85)
	at android.app.servertransaction.TransactionExecutor.executeCallbacks(TransactionExecutor.java:135)
	at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:95)
	at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2203)
	at android.os.Handler.dispatchMessage(Handler.java:106)
	at android.os.Looper.loop(Looper.java:268)
	at android.app.ActivityThread.main(ActivityThread.java:8017)
	at java.lang.reflect.Method.invoke(Native Method)
	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:627)
	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:997)
Caused by: java.lang.IllegalStateException: Not allowed to start service Intent { cmp=com.termux/.app.TermuxService }: app is in background uid UidRecord{3fb2066 u0a329 TPSL idle procs:1 seq(0,0,0)}
	at android.app.ContextImpl.startServiceCommon(ContextImpl.java:1831)
	at android.app.ContextImpl.startService(ContextImpl.java:1771)
	at android.content.ContextWrapper.startService(ContextWrapper.java:735)
	at com.termux.app.TermuxActivity.onCreate(TermuxActivity.java:242)
	at android.app.Activity.performCreate(Activity.java:8077)
	at android.app.Activity.performCreate(Activity.java:8061)
	at android.app.Instrumentation.callActivityOnCreate(Instrumentation.java:1315)
	at android.app.ActivityThread.performLaunchActivity(ActivityThread.java:3607)
	... 11 more

```
##


## Termux App Info

**APP_NAME**: `Termux`  
**PACKAGE_NAME**: `com.termux`  
**VERSION_NAME**: `0.118.0`  
**VERSION_CODE**: `118`  
**TARGET_SDK**: `28`  
**IS_DEBUGGABLE_BUILD**: `false`  
**APK_RELEASE**: `F-Droid`  
**SIGNING_CERTIFICATE_SHA256_DIGEST**: `228FB2CFE90831C1499EC3CCAF61E96E8E1CE70766B9474672CE427334D41C42`  
##


## Device Info

### Software

**OS_VERSION**: `4.14.186-00918-gb9b12c26f744-dirty`  
**SDK_INT**: `30`  
**RELEASE**: `11`  
**ID**: `RP1A.200720.011`  
**DISPLAY**: `X689-H696GHAa-R-GL-220210V564`  
**INCREMENTAL**: `220210V564`  
**SECURITY_PATCH**: `2022-02-05`  
**IS_DEBUGGABLE**: `0`  
**IS_TREBLE_ENABLED**: `true`  
**TYPE**: `user`  
**TAGS**: `release-keys`  

### Hardware

**MANUFACTURER**: `INFINIX MOBILITY LIMITED`  
**BRAND**: `Infinix`  
**MODEL**: `Infinix X689`  
**PRODUCT**: `X689-GL`  
**BOARD**: `Infinix-X689`  
**HARDWARE**: `mt6769`  
**DEVICE**: `Infinix-X689`  
**SUPPORTED_ABIS**: `arm64-v8a, armeabi-v7a, armeabi`  
##
