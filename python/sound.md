---
sort: 1
---

# 파이썬 기본음(sound) 출력

Mac OS 에서 사운드파일 다운로드 필요없이     
간단한 노티피케이션을 위한 비프음출력하기

    
   
    

### sound 목록 확인 
내 컴퓨터에서 기본으로 제공하는 sound 확인하기
1. 터미널을 연다
2. `ls /System/Libary/Sounds` 입력하기 
3. 확장자 명이 aiff 인 파일이 있는지 확인한다.


Basso.aiff      Blow.aiff       Bottle.aiff     Frog.aiff       Funk.aiff       Glass.aiff      Hero.aiff       Morse.aiff      Ping.aiff       Pop.aiff        Purr.aiff       Sosumi.aiff     Submarine.aiff  Tink.aiff
    
   
    

### 파이썬에서 코드 입력하기


```scss
import os

os.system('afplay /System/Library/Sounds/Submarine.aiff')

```

이렇게 하면 작은 비프음이 동작한다.
    
응용버전 
`os.system('say "please check"')` 이렇게 하면    
"플.리.즈. 체.크" 라고 또박또박 말해준다 ㅎ_ㅎ 파일이 없는데 간단한 노티알림음이 필요하시다면   
이렇게 해보시길 추천드립니당


