# Calculus

## 1. Single variable calculus
- Necessity
  - Differentiation(미분): 미분은 입력의 변화에 따라 출력이 얼마나 변화되는지 이해하는데 도움을 줌 → 값의 변화로부터 정보를 추출하는 방법
    - 딥러닝에서 순간적으로 값을 조금씩 learning rate를 변화시키며 최적의 솔루션을 찾는데 활용 → 이는 최적화(optimization)의 핵심 개념
  - Integration(적분): 적분은 특정 지점 간의 입력의 변화가 미치는 영향을 이해하는 데 도움을 줌
- Derivatives
  - Core Concepts
    - y = ±mx (±b)와 같은 직선 방정식이 있을 때, y는 x에 대한 함수이며, m은 직선의 기울기를 나타내며 b는 절편(원점으로부터 위나 아래로 얼마나 떨어져 있는지)을 나타냄
    - 이때, 직선의 기울기를 구하려면 m = (y2-y1) / (x2-x1)과 같이 구할 수 있음. 물론 이와 같이 단순한 직선의 경우 쉽게 기울기를 구할 수 있는데, 만약 함수가 연속적이어서 아래와 같이 곡선의 형태로 생겼다면?
    - <img height="300" src="https://github.com/PSLeon24/Calculus/assets/59058869/758d7530-e83e-4808-8737-07c92a6952fc">

    - 이를 위해서 함수의 도함수를 찾는 즉, 미분을 하면 됨. 미분을 한다는 것은 순간변화율을 찾는 것
      - ![image](https://github.com/PSLeon24/Calculus/assets/59058869/f4ba1a85-52e9-47aa-ad41-a76bdf172c94)
      - ![image](https://github.com/PSLeon24/Calculus/assets/59058869/8a5f2b33-cd1b-4ad9-9f81-b84f866505e3)

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
      - 곱의 미분법은 y = f(x)g(x)와 같이 두 함수의 곱으로 이루어진 식에 적용하는 미분법
      - F'(x) = f(x)g'(x) + f'(x)g(x) - 각각 하나씩 미분해서 더하기
    - Quotient rule
      - 몫의 미분법은 y = f(x)/g(x)와 같이 분수식으로 된 함수에 적용하는 미분법, 곱의 공식을 적용
      - F'(x) = (f(x)g'(x) - f'(x)g(x)) / g(x)^2
      - ![image](https://github.com/PSLeon24/Calculus/assets/59058869/84a20bdd-86b8-4e1c-a88e-77dcf7b95c3d)

    - Chain rule(합성함수의 미분)
      - 연쇄 법칙은 합성함수를 구성하는 각 함수의 미분의 곱으로 나타낼수 있다는 것
        - F'(x) = f'(g(x))g'(x)
        - 합성함수의 미분은 바깥함수(outer function)를 먼저 미분한 다음, 다시 안쪽 함수 (inner function)을 미분하여 곱하면 됨
        - 미분과 적분 전반에 걸쳐 사용되는 매우 중요한 미분법으로 여러 개의 함수가 미분가능하면 여러 개의 함수를 합성한 합성함수도 항상 미분이 가능하다는 것을 보여줌
        -  연쇄 법칙은 딥러닝의 Neural Network에서 사용되는 중요한 개념
        - ![image](https://github.com/PSLeon24/Calculus/assets/59058869/19d79e1d-914e-4a68-9277-e907bd45ec9a)
        - ![image](https://github.com/PSLeon24/Calculus/assets/59058869/b0725bab-730a-4a8e-b0c8-1adae07928e4)

    - Antiderivative
      - 부정적분은 이름 그대로 미분식 f'(x)를 통해 원래의 함수 f(x)를 찾는 역과정(마치 reverse engineering과 흡사한 과정)
      - 아래 이미지는 몇 개의 중요한 함수들의 부정적분을 정리한 표, 부정적분 후에는 임의의 상수 c를 붙여줘야 함
      - ![image](https://github.com/PSLeon24/Calculus/assets/59058869/7fb38218-e093-4d20-a527-54b9fd94c83c)


- Integrals
  - 적분은 미분과 정반대로 곡선 아래의 면적을 찾는 것, denoted by ∫(a,b)f(x)
    - ![image](https://github.com/PSLeon24/Calculus/assets/59058869/7761d2e8-bb58-46df-aa20-309a011a59b1)
  - 예를 들어 곡선 형태의 함수 f(x)가 있을 때, x가 a~b까지의 곡선 아래 면적은 아래와 같이 표기
    - ![image](https://github.com/PSLeon24/Calculus/assets/59058869/2490b65d-e92f-4de6-b062-457e640b47e2)
  - 또한, 극한을 활용해서 아주 작은 부분들의 면적의 합을 구하여 아래와 같이 나타낼 수도 있음
    - ![image](https://github.com/PSLeon24/Calculus/assets/59058869/09e25e8c-5855-476a-8a40-78b8e890599a)
    - ![image](https://github.com/PSLeon24/Calculus/assets/59058869/0a0e7570-d05e-4c91-aa34-d3bf873b31cb)
  - 수열의 규칙을 다루는 것은 적분을 구할 때 중요한 부분이고 깊게 이해하려면 수열의 규칙을 알아야 함
    - <img src="https://github.com/PSLeon24/Calculus/assets/59058869/8df122ec-8eb5-4ad3-8ac1-836e7cd68cb8" height="400">
  - 적분의 성질
    - ![image](https://github.com/PSLeon24/Calculus/assets/59058869/4a72a0be-2499-4852-8072-5f3df45f35f3)
    - ![image](https://github.com/PSLeon24/Calculus/assets/59058869/5ee92af7-0efa-44b7-a731-593c3b0a0a6e)

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
