# Calculus

## 1. Single variable calculus
- Necessity
  - Differentiation(미분): 미분은 입력의 변화에 따라 출력이 얼마나 변화되는지 이해하는데 도움을 줌
    - 딥 러닝에서 순간적으로 값을 조금씩 learning rate를 변화시키며 최적의 솔루션을 찾는데 활용 → 이는 최적화(optimization)의 핵심 개념
  - Integration(적분): 적분은 특정 지점 간의 입력의 변화가 미치는 영향을 이해하는 데 도움을 줌
- Derivatives
  - Core Concepts
    - y = ±mx (±b)와 같은 직선 방정식이 있을 때, y는 x에 대한 함수이며, m은 직선의 기울기를 나타내며 b는 절편(원점으로부터 위나 아래로 얼마나 떨어져 있는지)을 나타냄
    - 이때, 직선의 기울기를 구하려면 m = (y2-y1) / (x2-x1)과 같이 구할 수 있음. 물론 이와 같이 단순한 직선의 경우 쉽게 기울기를 구할 수 있는데, 만약 함수가 연속적이어서 아래와 같이 곡선의 형태로 생겼다면?
    - <img height="300" src="https://github.com/PSLeon24/Calculus/assets/59058869/758d7530-e83e-4808-8737-07c92a6952fc">

    - 이를 위해서 함수의 도함수를 찾는 즉, 미분을 하면 됨. 미분을 한다는 것은 순간변화율을 찾는 것
      - ![image](https://github.com/PSLeon24/Calculus/assets/59058869/f4ba1a85-52e9-47aa-ad41-a76bdf172c94)

    - 위와 같이 곡선이 있을 때 특정 지점에서 특정 지점까지의 거리가 h라고 가정하면 극한의 개념을 활용해서 다음과 같이 도함수를 구할 수 있음
      - fomular
        - ![image](https://github.com/PSLeon24/Calculus/assets/59058869/0cb5eedb-99f4-48df-9321-03b862013ec1)
    
  - Additional Concepts, Rules
    - Sum rule
      - 합의 법칙은 d/dx (f(x) + g(x))와 같이 두 함수를 합하여 미분한 것은 함수 각각을 미분하고 더한 값과 같음(뺄셈의 경우도 동일함)
      - ![image](https://github.com/PSLeon24/Calculus/assets/59058869/fe447b03-b90f-4e4b-9e51-394acee930b4)

    - Power rule
      - 멱의 법칙은 고등학교에서 학습한 내용과 같음. 오일러 상수(e)의 경우 미분해도 값이 그대로 나온다는 점도 기억
      - ![image](https://github.com/PSLeon24/Calculus/assets/59058869/3477d544-1634-4754-96a9-29b72a8e3730)

    - Trigonometric functions
      - ![image](https://github.com/PSLeon24/Calculus/assets/59058869/b9f7436a-4e54-4290-960d-51f9d53dc55c)

      - f(x) = sin(x)일 때, f'(x) = cos(x)이고, f(x) = cos(x)일 때, f'(x) = sin(x)

    - First and second derivatives
      - 첫 번째로 미분한 값, 즉, 도함수를 통해 함수의 gradient를 얻을 수 있고 이를 통해 얻을 수 있는 정보는 다음과 같음
        1. d/dx f(t) > 0: f(x)가 x=t일 때, 기울기는 양의 방향이다. 
        2. d/dx f(t) < 0: f(x)가 x=t일 때, 기울기는 음의 방향이다.
        3. d/dx f(t) = 0: f(x)가 x=t일 때, 기울기가 0, 즉, 극소값이나 극대값이라는 뜻이다.
      - second derivatives, 즉, 미분한 값에 한번 더 미분한 경우를 뜻하는데 이는 '이계도함수'를 뜻한다. 이는 도함수와 마찬가지로 함수가 증가하는지 감소하는지를 알려주며 추가로 함수의 복록성을 판단하는데 도움을 줌
        1. d^2/dx^2 f(t) > 0: 위로 볼록
           - 도함수가 0이면서 d^2/dx^2 f(t) > 0인 경우, f(x)는 x=t일 때 극댓값
        2. d^2/dx^2 f(t) < 0: 아래로 볼록
           - 도함수가 0이면서 d^2/dx^2 f(t) < 0인 경우, f(x)는 x=t일 때 극솟값
        3. d^2/dx^2 f(t) = 0: 변곡점을 구할 때도 쓰이지만 아무런 정보가 없을 수도 있음(변곡점인 것을 구하려면 주변의 도함수 값을 확인해봐야 함)
    - Product rule
      - 곱의 법칙
    - Quotient rule
      - 몫의 미분법
    - Chain rule
      - 연쇄 법칙
    - Antiderivative
      - 부정적분

- Integrals
  - The fundamental theorem of calculus
  - Substitution rule
  - Areas between curves
  - Integration by parts

## 2. Multivariable calculus
- Partial derivatives
  - Chain rule
- Integrals

## 3. Vector calculus
- Derivatives
- Vector fields
- Inverse functions

## Summary
