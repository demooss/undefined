# facile.js
Build web apps quickly and simply

~~웹 느려져도 Facile 문제 절대아님. 성능이수ㅠ없음. 그냥 없다 치셈~~

## 설치

### CDN
```
  https://cdn.jsdelivr.net/gh/demooss/Facile@1.0.0/dist/facile.js
```
그냥 자바스크립트 가져오는것 처럼 똑같이 가져오세요.

어디 둬도 상관 없는데 그냥 head 태그 안에 두세요
```html
  ...
  <head>
    <script src="./index.js"></script>
  </head>
  ...
```
이렇게.

## 데이터 바인딩
그냥 따라치세요.
```html
     <p>{{ op.t }}</p>

    <script>
        let op = {
            t:"어머나 세상에"
        }
    </script>
```
이렇게 치면 당연히 `{{ op.t }}` 부분에 `어머나 세상에` 가 들어가지않을까요

**+2022년 8월 25일 업데이트**
> 기존에는 전체 DOM이 수정되었지만 이제는 변경된 부분만 바뀝니다

## 더하기
```html
  <p>{{ 1+2 }}</p>
```
수학 잘 하시면 `{{ 1+2 }}` 부분에 뭐가 들어갈지 당연히 아실꺼에요

## 인풋 Value 바인딩
첫번째 인풋에 쓴거랑 두번째 인풋에 쓴것을 더해봅시다
```html
    <input type="text" bind-value="test1">
    <input type="text" bind-value="test2">

    <p>{{ test1+test2 }}</p>
```

**+ 2022년 8월 25일 업데이트**
> 꼭 input의 타입을 해당 인풋에 쓸 내용에 맞게 넣으세요.
> 
> 예를들어 숫자만 입력할꺼면 `number`로 해주시고, 글자와 숫자가 같이 입력될꺼면 `text`로 해주세요.
> 
> 만약 타입이 다르면 오류가 날수도 있어요.

## 그냥 아무거나 해보세요
~~사실 `{{ }}` 안에 js 코드 아무거나 넣어도 다 실행 됩니다~~
**+ 2022년 8월 25일 업데이트**
> 더이상 `{{ }}` 안에서 js코드를 사용할 수 없어요
> 
> `{{ }}`안에서는 데이터 바인딩만 가능해요

## 불친절한 문서
돈이 안되서 그냥 불친절하게 할껍니다

## 기능 요청
만든지 2일된거에 뭘 더 요구하시게요

필요하면 이슈나 남기세요.
