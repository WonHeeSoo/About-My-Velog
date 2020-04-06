[Xcode] duplicate symbol 문제 해결하기

# 🧱 사양

**Xcode 10.1**

# 💣 문제
외부 SDK를 추가하는 과정에서 오류가 발생했습니다.
가이드 대로 **`Other Liner Flags`**에 **`-all_load`** 추가했지만 여러 외부 Framework를 사용하다 보니 Framework간에 충돌이 일어났습니다. 게다가 **`duplicate symbol`** 메시지가 정말 많아서 한 두개 수정할 문제는 아니였습니다.

### ❗ Error
```java
  duplicate symbol...
  duplicate symbol...
  duplicate symbol...
  duplicate symbol...
```

# 💡 해결
일반적으로 **'-all_load'** 대신 **'force_load'**를 사용해 해결하는 방법이 많았으나 다른 방법을 사용했습니다.

![이미지](https://github.com/WonHeeSoo/About-My-Velog/blob/master/Images/Xcode/Duplicate%20Symbol%20Framework%20Path.png?raw=true)

**Build Settings**의 **Framework Search Paths**에 추가할 **framwork의 경로**를 추가하였습니다.

