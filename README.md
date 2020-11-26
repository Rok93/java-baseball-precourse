# 미션 - 숫자 야구 게임

## 🎯 구현할 기능 목록 

> 기능 구현표는 중간에 추가 혹은 삭제될 수 있습니다.  

- [x] 숫자야구게임에서 각 자리숫자 역할을 하는 기능 (BaseballNumber 객체) ⚙️ 
    - [x] 1 ~ 9 이외의 숫자를 입력받을 경우 예외 발생 🚨
- [x] 숫자야구게임에서 세자리의 수 역할을 하는 기능 (BaseballNumbers 객체) ⚙️
    - [x] 중복된 숫자를 입력받은 경우 예외 발생 🚨 
    - [x] 입력받은 숫자가 세자리수가 아닌 경우 예외 발생 🚨
- [x] 1에서 9까지의 숫자 중에서 서로 다른 임의의 수 3개를 입력받는 기능 ⚙️
    - [x] 숫자 대신 문자를 입력받을 경우 예외 발생 🚨 
- [x] 1에서 9까지의 숫자 중에서 서로 다른 임의의 수 3개를 생성하는 기능 ⚙️
- [x] 숫자야구 게임을 실행하는 기능 ⚙️
- [x] 스트라이크 개수를 구하는 기능 ⚙️
- [x] 볼 개수를 구하는 기능  ⚙️
- [ ] 힌트를 출력하는 기능 ⚙️
- [ ] 게임을 재시작 or 종료하는 기능 ⚙️   
    - [ ] 1, 2 이외의 숫자를 입력받을 경우 예외 발생 🚨 

## ✅ 프로그래밍 요구사항
> 1차적으로 기능구현이 끝나면 이 요구사항들을 잘 지켰는지 확인한다. 

### General 
- [ ] 자바 코드 컨벤션을 지키면서 프로그래밍한다.
- [ ] indent(인덴트, 들여쓰기) depth를 3이 넘지 않도록 구현한다. 2까지만 허용한다.
- [ ] 3항 연산자를 쓰지 않는다.
- [ ] 함수(또는 메소드)가 한 가지 일만 하도록 최대한 작게 만들어라.
- [ ] System.exit 메소드를 사용하지 않는다.
- [ ] 비정상적 입력에 대해서는 IllegalArgumentException을 발생시킨다.

### Application 
- [ ] Application 클래스를 활용해 구현해야 한다.
- [ ] Application의 패키지 구조와 구현은 변경하지 않는다.
- [ ] `final Scanner scanner = new Scanner(System.in);`는 변경하지 않는다.
- [ ] `// TODO 구현 진행` 이 후 부터 구현한다.

### RandomUtils
- [ ] RandomUtils 클래스를 활용해 랜덤 기능을 구현해야 한다.
- [ ] RandomUtils의 패키지 구조와 구현은 변경하지 않는다.

## 🤔 고민한 부분 
* 숫자 대신 문자를 입력받을 경우 예외 
> 문자열입력을 받아. 한글자씩 분리하고 Integer type으로 변경하여 List를 만들 예정 
> 숫자가 아닌 문자가 있을 경우 변환과정에서 NumberFormatException이 발생한다. 
> NumberFormatException은 IllegalArgumentException를 상속받기 때문에  
> 단순히 IllegalArgumentException을 catch 해줌으로써, 예외처리를 할 수 있다! 
