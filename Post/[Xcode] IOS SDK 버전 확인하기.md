[Xcode] IOS SDK 버전 확인하기

# 💡 1. 공식 홈페이지

[Apple Developer Xcode Release Notes](https://developer.apple.com/documentation/xcode_release_notes)

Topics에서 자신의 Xcode 버전에 맞는 Release Notes로 들어갑니다.
Overview에 Xcode에 포함된 SDK version을 확인합니다.


# 💡 2. 시스템 리포트

`이 Mac에 관하여` -> `시스템 리포트` -> `소프트웨어` -> `개발자`
![사진](https://github.com/WonHeeSoo/About-My-Velog/blob/master/Images/Xcode/IOS%20SDK%20Version.png?raw=true)

# 💡 3. 터미널
Xcode가 여러 버전이 설치되어 있을 경우 기본으로 설정되어 있는 Xcode의 SDK 버전이 표기된다.

```bash
xcodebuild -showsdks
```

![사진](https://github.com/WonHeeSoo/About-My-Velog/blob/master/Images/Xcode/Bash%20IOS%20SDK%20Version.png?raw=true)
