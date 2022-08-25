# reset.css와 normalize.css

우선 위와 같은 Reset.css와 Normalize.css를 사용하는 이유는 웹 브라우저마다 기본 스타일을 제공하기 때문이다.

그래서 내가 짠 스타일처럼 나오지 않는 것을 방지하려면 스타일을 초기화 하는 코드를 넣어줘야 한다.

## Reset.css

브라우저 간의 차이를 최대한 없애는 코드를 넣어서, 브라우저 요소들의 스타일이 0인 상태에서 디자인을 만들어 나가기 위해 생긴 코드이다.

[meyerweb.com](https://meyerweb.com/eric/tools/css/reset/)

## Normalize.css

reset.css와 조금 다르며, 약간의 디자인적인 요소가 가미되어 있다.

[Normalize.css](https://necolas.github.io/normalize.css/)

reset.css는 완전 스타일을 초기화 해주는 코드고, normalize.css는 스타일을 초기화 해주면서 약간의 디자인이 들어간 코드이다.

## 적용 방법

- 외부 스타일 시트 적용
  ```css
  <head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="reset.css">
    <link rel="stylesheet" href="normalize.css">
    <title>Document</title>
  </head>
  ```
