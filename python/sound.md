---
sort: 3
---

# 파이썬 기본음(sound) 출력

Mac OS 에서 사운드파일 다운로드 필요없이 
간단한 노티피케이션을 위한 비프음출력하기


## sound 목록 확인 
내 컴퓨터에서 기본으로 제공하는 sound 확인하기
1. 터미널을 연다
2. `ls /System/Libary/Sounds` 입력하기 
3. 확장자 명이 aiff 인 파일이 있는지 확인한다.

Basso.aiff      Blow.aiff       Bottle.aiff     Frog.aiff       Funk.aiff       Glass.aiff      Hero.aiff       Morse.aiff      Ping.aiff       Pop.aiff        Purr.aiff       Sosumi.aiff     Submarine.aiff  Tink.aiff

## 파이썬에서 코드 입력하기

```
import os

os.system('say "please check"')
os.system('afplay /System/Library/Sounds/Submarine.aiff')

```

**Highlight:**

```scss
import os

os.system('say "please check"')
os.system('afplay /System/Library/Sounds/Submarine.aiff')

```
