# 기능 목록

## Model

- 무작위 로또 번호를 생성한다.
- 입력받은 로또 번호와 무작위로 생성된 로또 번호를 대조한다.

  **입력 값 검증**

  - 숫자가 아닌 경우
  - 쉼표 기준으로 나누어진 숫자가 6개가 아닌 경우
  - 로또 번호가 1에서 45 사이의 수가 아닌경우

- 대조 결과에 따른 결과를 반환한다.

  **당첨 결과**

  - 1등: 6개 번호 일치 / 2,000,000,000원
  - 2등: 5개 번호 + 보너스 번호 일치 / 30,000,000원
  - 3등: 5개 번호 일치 / 1,500,000원
  - 4등: 4개 번호 일치 / 50,000원
  - 5등: 3개 번호 일치 / 5,000원

## Controller

- 로또 구입 금액 입력값을 검증한다.

  **예외 케이스**

  - 숫자가 아닌경우
  - 1,000 단위의 금액이 아닌 경우

- 당첨 번호 입력 값을 검증한다.

  **예외 케이스**

  - 입력 값에 쉼표가 없는 경우

- 보너스 번호 입력 값을 검증한다.

  **예외 케이스**

  - 숫자가 아닌 경우

## View

### InputView

- 로또 구입 금액을 입력받는다.
- 로또 당첨 번호를 입력받는다.
- 로또 보너스 번호를 입력받는다.

### OutputView

- 구매한 로또들의 번호를 출력한다.
- 구입금액과 당첨금을 비교해 수익률을 계산하고, 당첨 통계를 출력한다.
