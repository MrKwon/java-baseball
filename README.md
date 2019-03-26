# 1주차 미션 야구게임(java-baseball)

## 기능 요구사항
- 1부터 9까지 서로 다른 수로 이루어진 3자리의 수를 맞추는 게임
- 같은 수가 같은 자리에 있으면 스트라이크
- 같은 수가 다른 자리에 있으면 볼
- 같은 수가 전혀 없으면 포볼 또는 낫싱 (힌트)

- 컴퓨터가 상대방, 유저가 플레이어
- 컴퓨터는 **서로 다른 임의의 수 3개**를 선택
- 플레이어는 컴퓨터가 생각하고 있는 3개의 숫자를 입력
- 컴퓨터는 입력한 숫자에 대한 결과를 출력

- 이 과정을 반복해 컴퓨터가 선택한 3개의 숫자를 모두 맞히면 게임이 종료
- 게임을 종료한 후 게임을 다시 시작하거나 완전히 종료할 수 있음

## 프로그램 요구사항
- [자바 코드 컨벤션](https://myeonguni.tistory.com/1596)을 지키면서 프로그래밍
- Indent depth 가 3이 넘지 않도록 한다
- 함수나 메서드가 한가지 역할만 하도록 최대한 작게 만든다.

## 구현할 기능 목록
1. ``gameInit()`` - 서로 다른 임의의 숫자 3개를 만들어 ~~String 으로 반환~~ int[]로 반환하는 메서드
2. ``getUserInput()`` - 사용자의 입력을 받는 메서드
3. ``countStrike(int[] com, int[] user)`` - 사용자의 입력과 숫자 3개를 비교하여 스트라이크를 count 하는 메서드
3. ``countBall(int[] com, int[] user)`` - 사용자의 입력과 숫자 3개를 비교하여 볼을 count 하는 메서드
~~4. 3번의 count 를 출력하는 함수~~
4. ``printGameResult(int strike, int ball)`` - 스트라이크와 볼의 결과에 맞게 결과 문자열을 콘솔에 출력하는 메서드
5. ``gameStart(int[] com)`` - 3개의 숫자를 모두 맞힐 때까지 반복하는 몸통 메서드
6. ``isGameEnd(int strike)`` - 게임이 끝났는지 아닌지를 반환해주는 메서드
- (추가 혹은 수정이 필요할 경우 수정)

## 개발 일지
1. 기능만 구현하는 스파게티 코드로 작성
2. 1차 리팩토링, 모든 기능 함수화
3. 2차 리팩토링, 진행중. 객체지향의 특성에 맞게 리팩토링