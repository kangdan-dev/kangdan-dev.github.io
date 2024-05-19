---
sort: 1
---

# 안드로이드 스톱워치 만들기
굉장히 기본적인 스톱워치 앱을 만들어보도록 하겠습니다.   
디자인은.. 없습니다.     
기본적이고 베이직한 UI이니까 import 받으셔서 커스텀해보시면 좋을거같아요 ^-^   
https://github.com/kangdan-dev/android.git       
app 모듈에 있습니다~   




## 리사이클러 뷰 기초
안드로이드에서 목록(리스트)를 보여줄 때 사용합니다.

### 리사이클러 뷰 구성요소
- ViewHolder : 뷰 객체
- Adapter : 항목구성
- LayoutManager : 항목배치
- (선택적으로) ItemDecoration : 꾸미기    
              
          
            
## 예시로 쉽게 이해하기 
                  
#### ✻ ViewHolder
뷰홀더는 뷰 객체들로 구성되어있습니다.     
텍스트뷰, 이미지뷰, 버튼 등을 이용&배치하여 데이터들이 어떻게 보여질지 정합니다.    
     
뷰홀더는 틀(붕어빵틀)     
어댑터는 재료(팥, 슈 등)    
이라고 이해하시면 쉽습니다.     

예를들어,     
"게시판 공지사항" 목록을 리사이클러뷰로 만들어본다면    
먼저 목록에 어떤 정보가 보여질지 정해야합니다.    

신규여부, 제목, 내용, 날짜, 작성자가 있도록 보여주고싶다면    
<img width="301" alt="스크린샷 2024-05-19 오후 4 49 37" src="https://github.com/kangdan-dev/kangdan-dev.github.io/assets/17777689/c018b608-17ca-4bd8-ace4-3464a7686103">      
이러한 모습이 되겠죠. 

목록을 레이아웃으로 그린다면      
<img width="458" alt="스크린샷 2024-05-19 오후 4 50 42" src="https://github.com/kangdan-dev/kangdan-dev.github.io/assets/17777689/fed258da-f668-496c-8058-5db38fd21af2">      
아마도 이런배치일것같습니다.     

이것이 뷰홀더입니다.   

#### ✻ Adapter
어댑터는 뷰홀더에 데이터를 대입합니다.

저 뷰 홀더에 각각 데이터를 지정하여 대입해줍니다.     
ex) titleTextView.text = datas[position]     //값을 세팅 




