# 자동차 경주 게임
## 기능 요구사항
* 초간단 자동차 경주 게임을 구현한다.
* 주어진 횟수 동안 n대의 자동차는 전진 또는 멈출 수 있다.
* 사용자는 몇 대의 자동차로 몇 번의 이동을 할 것인지를 입력할 수 있어야 한다.
* 전진하는 조건은 0에서 9 사이에서 random 값을 구한 후 random 값이 4이상일 경우이다.
* 자동차의 상태를 화면에 출력한다. 어느 시점에 출력할 것인지에 대한 제약은 없다

## 프로그래밍 요구사항
* 모든 로직에 단위 테스트를 구현한다. 단, UI(System.out, System.in) 로직은 제외
    * 핵심 로직을 구현하는 코드와 UI를 담당하는 로직을 구분한다.
    * UI 로직을 InputView, ResultView와 같은 클래스를 추가해 분리한다.
* 자바 코드 컨벤션을 지키면서 프로그래밍한다.
    * 참고문서: https://google.github.io/styleguide/javaguide.html 또는 https://myeonguni.tistory.com/1596
* else 예약어를 쓰지 않는다.
    * 힌트: if 조건절에서 값ResultPrint을 return하는 방식으로 구현하면 else를 사용하지 않아도 된다.
    * else를 쓰지 말라고 하니 switch/case로 구현하는 경우가 있는데 switch/case도 허용하지 않는다.
 
 ## 기능목록
 * RunCarRace -- 레이싱 시작 관리 클래스
    * run() - 레이싱 시작
    * inputValue() - 파라미터를 받는 메소드
    * repeatTryMoveCar() - 시동할 횟수를 반복
    * repeatCar - 자동차 갯수를 반복
 * CarRaceInformation -- 자동차의 정보 관리 클래스
    * 자동차의 댓수와, 이동시도횟수, 자동차 댓수에 따른 이동횟수 배열
 * NumberInput - 입력받은 값 체크 클래스
    * inputCount : 키보드로 input값 받기
    * valueCheck : 키보드로 임력받은 값 체크 (null, empty, arrayException 처리)
 * ResultPrint - 자동차 그리는 관리 클래스
    * drawMoveCar : 자동차의 이동한 배열을 받아 그려주는 메소드
 * Car - 자동차의 이동 여부 관리 클래스
 * ErrorMessage : 에러메세지 관리 클래스

           
                  
 
## 온라인 코드 리뷰 과정
* [텍스트와 이미지로 살펴보는 온라인 코드 리뷰 과정](https://github.com/next-step/nextstep-docs/tree/master/codereview)
