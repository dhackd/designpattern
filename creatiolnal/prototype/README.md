**prototype**<br>
목적
- 객체를 생성함에 있어서 기존의 초기화된 값을 그대로 가지고 복제받기를 원할때 사용할 수 있다.<br>

장점
- new 연산자를 통해서 객체를 생성할때 값이 초기화 되지만
prototype일경우엔 생성자를 통해 이미 세팅된 값이 그대로 복제되기 때문에
원하는 값만 setter()를 변경할 수 있음으로써 수고를 덜 수 있다.

고려사항
- 만약 필드값중 객체를 사용하는 것이 있다면?

깊은복사
- 객체가 가지는 값 자체를 모두 복사하게 됨.

얕은복사
- 참조복사로 주소값이 변경되므로 이때 setter를 통해서 특정 필드 값을 
변경할때 original 값도 같이 변경이 된다는점...