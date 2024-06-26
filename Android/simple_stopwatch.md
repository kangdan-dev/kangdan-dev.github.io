---
sort: 2
---
               
# 리사이클러 뷰 기초
안드로이드에서 목록(리스트)를 보여줄 때 사용합니다.

### 리사이클러 뷰 구성요소
- ViewHolder : 뷰 객체
- Adapter : 항목구성
- LayoutManager : 항목배치
- (선택적으로) ItemDecoration : 꾸미기    
                
&nbsp;  




## 예시로 쉽게 이해하기 
####  > viewHolder  
<span style="font-size:70%">
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
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;

  
목록을 레이아웃으로 그린다면      
<img width="458" alt="스크린샷 2024-05-19 오후 4 50 42" src="https://github.com/kangdan-dev/kangdan-dev.github.io/assets/17777689/fed258da-f668-496c-8058-5db38fd21af2">      
아마도 이런배치일것같습니다.     
&nbsp;      
이것이 뷰홀더입니다.   </span>       
   
     
     
                      
#### > Adapter

자~ 그림은 그렸고 이제 그림에 데이터를 넣어볼까요?
어댑터는 뷰홀더에 데이터를 **대입**합니다.      
           
저 뷰 홀더에 각각 데이터를 지정하여 대입해줍니다.       
ex)   
```scss
class SampleAdapter () {  
      textview.setText("00:00:00");    //대입   
}  
```
                 

## 자세한건 코드로!
https://github.com/kangdan-dev/android   
이 프로젝트를 import해서 app모듈을 확인해보자!!  





