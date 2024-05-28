---
sort: 1
---

# Toast message      
토스트T 메시지ToastMessage는 화면 아래쪽에 약 2초간 나타났다가 사라지는 메시지를 뜻합니다.   
보통은 "종료하려면 한번 더 누르세요" 와 같은 문구 많이들 보셨을 겁니다~   




## 기본문법          
Toast는 makeText()함수로 만듭니다.        
makeText(context, Text, duration)      
              
이 기본 문법입니다.      
매개변수를 차근차근 살펴볼까요?       
                
         
> context : this       
> Text : 보여줄 메시지              
> duration : 나타낼 시간


                
Toast.makeText(this, "종료하려면 한번 더 누르세요" , Toast.LENGTH_SHORT).show()


### daration
안드로이드에선 친절하게도 duration을 함수로 편리하게 제공합니다.          
Toast.LENGTH_SHORT : 3초          
Toast.LENGTH_LONG : 5초        
                          
                         
## Toast callback감지
토스트는 콜백이 필요없을정도의 간단한 메시지를 노출하지만       
때로는 토스트가 사라지는 시점을 감지할 필요가 있겠지요?!     
            


               
콜백은 API30이상에서만 가능합니다!!    

```javascript    
val toast = Toast.makeText(this, "토스트메시지 입니다.", Toast.LENGTH_SHORT)    
toast.addCallback(     
     object : Toast.Callback(){
          override fun onToastHidden(){
              super.onToastHidden()
              //TODO toast hidden...
          }
          override fun onToastShown(){
              super.onToastShown()
              //TODO toast shown...
          }
      })
toast.show()
```





화면에 토스트가 뜨는 순간 자동으로 콜백 객체의 onToastShown()함수가 호출되며,    
화면에서 토스트가 사라지는 순간 자동으로 OnToastHidden()함수가 호출됩니다.             




                                        
                       
           
