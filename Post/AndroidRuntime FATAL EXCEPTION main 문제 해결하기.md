[Android Studio] E/AndroidRuntime: FATAL EXCEPTION: main 문제 해결하기

# 💣 문제
외부 SDK를 추가하는 과정에서 오류가 발생했습니다.
Error 내용에 친절하게 가이드가 있는 오류입니다.

### ❗ Error
```java
    E/AndroidRuntime: FATAL EXCEPTION: main
    java.lang.RuntimeException: Unable to get provider com.google.android.gms.ads.MobileAdsInitProvider: java.lang.IllegalStateException: 
    
    ******************************************************************************
    * The Google Mobile Ads SDK was initialized incorrectly. AdMob publishers    *
    * should follow the instructions here: https://goo.gl/fQ2neu to add a valid  *
    * App ID inside the AndroidManifest. Google Ad Manager publishers should     *
    * follow instructions here: https://goo.gl/h17b6x.                           *
    ******************************************************************************
```

# 💡 해결

### 🛠 공통 사전 작업

```
allprojects {
    repositories {
        google()
        jcenter()
    }
}
```

```
dependencies {
    implementation 'com.google.android.gms:play-services-ads:18.3.0' // 버전 확인 필요
}
```

&nbsp;

### 🛠 AdMob의 경우
```xml
<manifest>
    <application>
        <meta-data
            android:name="com.google.android.gms.ads.APPLICATION_ID"
            android:value="ca-app-pub-3940256099942544~3347511713"/> // 자신의 AdMob App ID
    </application>
</manifest>
```
android:value에는 자신의 AdMob App ID를 넣으면 됩니다.
[AdMob 관련 페이지](https://developers.google.com/admob/android/quick-start#update_your_androidmanifestxml)

&nbsp;

### 🛠 Google Ad Manager의 경우
```xml
<manifest>
    <application>
        <meta-data
            android:name="com.google.android.gms.ads.AD_MANAGER_APP"
            android:value="true"/>
    </application>
</manifest>
```
[Google Ad Manager 관련 페이지](https://developers.google.com/ad-manager/mobile-ads-sdk/android/quick-start#update_your_androidmanifestxml)