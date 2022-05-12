# 22.05.12  
타입스크립트를 왜 쓸까?  
자바스크립트의 경우 타입에의한 에러를 잡아줄수 없다 때문에 바로잡기 위해 타입스크립트 사용!

타입스크립트로 작성하고 왜 다시 자바 스크립트로 변환?  
브라우저는 타입스크립트를 해석할 수 없기때문에 자바스크립트로 변환해줍니다.  
(Node.js는 둘다 가능)

타입스크립트는 변수의 타입을 지정해주고 Type checker를 통해 확인합니다.

타입  
readonly - 수정하지 못하게 보호해준다.  
unknown - 변수의 타입을 알지못할때  
void - 아무것도 return 하지 않을때 (비어있는것을 뜻하며 타입을 따로 지정해주지않아도된다.)  
never - 함수가 return 하지않을때

<br></br>

# 22.05.13
CallSignature
  - 타입을 직접 만들고 함수가 어떻게 작동할지 서술하여 사용  
ex) type Add = (a : number, b : number) => number  
const add:Add = (a, b) => a+b

Overloding
  - 함수가 여러개의 다른 CallSignature를 가지고 있을때 발생  

Polymorphism(다형성)
  - 여러 CallSiignature 사용가능

Generic
  - 요구한대로 CallSignature생성하는 도구
  - 타입 재사용 가능
