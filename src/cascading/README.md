# cascading

cascading은 폭포라는 의미를 가지고 있음

우선순위를 중요시 여김

### 우선순위

인라인 스타일로 입력한 값 > ID로 입력한 값 > Class로 입력한 값 > 스타일에서 가장 마지막에 입력한 값 >시멘틱 태그

![ezgif.com-gif-maker.gif](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/3ebcd52a-dfe7-43ae-8dcc-4850c7110421/ezgif.com-gif-maker.gif)

```html
<body>
  <div class="center">
    <ul>
      <li>item 01</li>
      <li id="id_selector" class="class_selector">item 02</li>
      <li class="class_selector">item 03</li>
      <li>item 04</li>
    </ul>
  </div>
</body>
```

1. item 01, item 02, item 03, item 04는 li 태그로 배경 파란색을 줌

   ```css
   li {
     padding: 10px;
     margin: 10px;
     width: 120px;
     height: 50px;
     line-height: 50px;
     border-radius: 8px;
     text-align: center;
     font-size: 16px;
     color: #fff;
     background: #004fff; //파란색
   }
   ```

2. item 02, item 03은 class로 배경 초록색을 줌

   ```css
   .class_selector {
     background: green;
   }
   ```

3. item 02는 id 값으로 배경 빨간색을 줌

   ```css
   #id_selector {
     background: red;
   }
   ```

4. item 02를 인라인 스타일로 배경 노란색을 줌

   ```html
   <li id="id_selector" class="class_selector" style="background-color: yellow">
     item 02
   </li>
   ```

5. item 01, item 04의 li 태그를 마지막에 추가하여 값으로 배경 검정색을 줌

   ```css
   li {
     padding: 10px;
     margin: 10px;
     width: 120px;
     height: 50px;
     line-height: 50px;
     border-radius: 8px;
     text-align: center;
     font-size: 16px;
     color: #fff;
     background: #004fff; // 파란색
   }
   li {
     background: black; // 검정색 마지막에 추가된 li 태그가 적용됨
   }
   ```
