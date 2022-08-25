# 부모와 자식 관계

```html
<article>
  <h1>제목</h1>
  <p>설명</p>
</article>
```

이렇게 코드가 있다면, h1 태그는 article 태그의 자식이다.

반대로 article은 h1 태그의 부모이다.

이렇게 html은 부모와 자식 관계로 이루어져 있다.

## 스타일 입히는 방법

```html
<div class="container">
  <h1>리스트</h1>
  <article>
    <h1>제목</h1>
    <p>설명</p>
  </article>

  <article class="dark-mode">
    <h1>제목</h1>
    <p>설명</p>
  </article>

  <article>
    <div class="title">
      <h1>제목</h1>
    </div>

    <p>설명</p>
  </article>
</div>
```

이렇게 코드가 주어졌다.

- 클래스 container에 스타일 입히기
  ```css
  .container {
    width: 100%;
    max-width: 1080px;
    padding: 40px;
    margin: auto;
  }
  ```
- 모든 article 태그와 h1태그에 스타일 입히기
  ```css
  article {
    width: 100%;
    padding: 20px;
    font-size: 16px;
    background-color: #eee;
    border-radius: 10px;
    margin-bottom: 20px;
  }

  h1 {
    font-size: 24px;
    margin-bottom: 10px;
  }
  ```
- 그 중 article 태그 바로 하위에 있는 h1 태그에 스타일 입히기
  ```css
  /* article 태그의 바로 하위에 있는 h1 태그를 가리킨다. */
  article > h1 {
    font-size: 20px;
    margin: 0;
  }
  ```
  > 바로 하위를 가리킬 때는 `>` 를 사용해준다.
- article 태그 하위 모든 p 태그에 스타일 입히기
  ```css
  article p {
    margin: 0;
  }
  ```
- 클래스 dark-mode에 스타일 입히기
  ```css
  .dark-mode {
    background-color: black;
  }

  .dark-mode h1,
  .dark-mode p {
    color: #eee;
  }
  ```

## 위 코드 결과

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/95f01e63-f3ad-4547-acdf-e720a65ac499/Untitled.png)
