[Mac] 외장하드 파티션 버튼이 비활성화일 때 해결하기

# 🧱 사양

**Mac OS Mojave**

# 💣 문제

![이미지](https://github.com/WonHeeSoo/About-My-Velog/blob/master/Images/Mac%20Disk%20Utility/External%20Hard%20Drive%20No%20Partition01.png?raw=true)

**외장하드**를 **파티션**을 나누려고 했으나 **비활성화 상태**였습니다.

# 💡 해결

1. **command**창을 열어 **문제가 되는 외장 디스크의 이름을 확인**합니다.

```bash
diskutil list
```

![이미지](https://github.com/WonHeeSoo/About-My-Velog/blob/master/Images/Mac%20Disk%20Utility/External%20Hard%20Drive%20No%20Partition02.png?raw=true)

**internal**이 **내장**, **external**이 **외장 하드** 이므로 **disk3**이 **외장하드**입니다.
**파티션**을 나눌 수 있도록 **외장하드**를 **포맷**해야 합니다.

---

2. **command**창에서 **외장하드**인 **disk3**를 **포맷**합니다.

```bash
sudo diskutil partitionDisk disk3 GPT JHFS+ one 0GB
```

![이미지](https://github.com/WonHeeSoo/About-My-Velog/blob/master/Images/Mac%20Disk%20Utility/External%20Hard%20Drive%20No%20Partition03.png?raw=true)

---

3. **디스크 유틸리티**에서 **파티션 버튼**이 **활성화** 되었는지 **확인**합니다.

![이미지](https://github.com/WonHeeSoo/About-My-Velog/blob/master/Images/Mac%20Disk%20Utility/External%20Hard%20Drive%20No%20Partition04.png?raw=true)

