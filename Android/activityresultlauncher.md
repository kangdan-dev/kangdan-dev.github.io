---
sort: 3
---

# ActicityResultLauncher      
예전엔 startActivityForResult를 통해     
액티비티 전환 사후처리를 했으나, 요즘은 권장하지 않습니다.   
그럼 뭘 쓰느냐~   
바로 ActicityResultLauncher를 사용합니다.
</br>  
</br>  
</br>  

```ActicityResultLauncher 생성   
val requestLauncher : ActicityResultLauncher<Intent> = registerForActivityResult(ActivityResultContracts.StartActivityForResult()){      
    val resultData = it.data?getStringExtra("result")    
    Log.i("LOG resultdata = $resultData");    
}

...    

val intent:Intent = Intent(this, A::class.java)     
requestLauncher.launch(intent)    

```
</br>  
</br>  

### 자세히 살펴보기
ActivityResultLauncher 이용하려면 먼저       
> 1. ActicityResultLauncher 객체 만들기 (registerForActivityResult() 이용하기)     
>         
> 2. 1번 객체에 contract와 callback 등록하기
>    
> 3. launch()함수로 실행              

                
#### Contract가 뭐지?
액티비티를 실행할때 인텐트를 발생시키는 역할을 합니다.   
대표적인 Contract는   
* RequestPermission : 권한요청, 허락여부파악
* PickContact : 선택한 연락처의 Uri 획득
* TackPicture : 사진촬영, 저장, 비트맵
-- * StartActivityForResult : 인텐트발생, 액티비티 실행결과 획득 --

  </br>  
  </br>  
  </br>  
  





