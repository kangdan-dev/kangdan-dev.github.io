---
sort: 1
---

# 파이썬 기본음(sound) 출력

Mac OS 에서 사운드파일 다운로드 필요없이     
간단한 노티피케이션을 위한 비프음을 출력해볼까합니다.   
     
단 두줄만에 가능하니 쉽게 구현가능하실겁니다.


```scss
import os

os.system('say "please check"')

```

이렇게 하시면 따옴표 안에 있는 글자를 읽어줍니다.   
'say' 라는 단어 보이시죠? 얘 덕분에 뒤에 있는 글자를 출력해주는겁니다.    

이게 약간 허접..해보일수있습니다 ㅠㅠ    
    
그래서 맥에서 기본으로 제공해주는 간단한 비프음도 출력해볼까요.    



     

## sound 목록 확인 
내 컴퓨터에서 기본으로 제공하는 sound 확인하기
1. 터미널을 연다
2. `ls /System/Libary/Sounds` 입력하기 
3. 확장자 명이 aiff 인 파일이 있는지 확인한다.
    

<span style="font-size:75%"> Basso.aiff      Blow.aiff       Bottle.aiff     Frog.aiff       Funk.aiff       Glass.aiff      Hero.aiff       Morse.aiff      Ping.aiff       Pop.aiff        Purr.aiff       Sosumi.aiff     Submarine.aiff  Tink.aiff </span>

      
      
      
    
## 파이썬에서 코드 입력하기


```scss
import os

os.system('afplay /System/Library/Sounds/Submarine.aiff')

```

이렇게 하면 작은 비프음이 동작합니다.    

   끝 ㅎㅎ


    

