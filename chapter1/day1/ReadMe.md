##### 2022-06-25
##### chapter1 day1 [0 ~ 16]

# 예상을 빗나가는 코드
위와 같은 방식의 코드를 작성할 경우 코드가 우리의 상식과는 다르게 동작하기 때문에 이해하기 어려운 코드가 된다.  
문제는 Theater클래스의 enter메소드이다. enter메소드에서 판매원과 고객을 마음대로 접근하고 있기 때문이다.  
쉽게 얘기하자면 현실 세계에서 제 3자가 고객의 가방을 탈취해 돈을 마음대로 지불하고 티켓을 구매하는 것이다. 판매자 입장에서도 판매를 원하건 말건 제 3자가 마음대로 티켓을 판매해 버리는 것이다.  

# 변경에 취약한 코드
가장 큰 문제는 Theater객체가 Audience와 TicketSeller에 의존적이다. 이 두 클래스의 변경이 생기면 Theater클래스도 변경 되어야 한다는 문제가 있다.
