# 저는 오늘 이런 것들을 했어요!! 😎

## 오늘 열심히 공부한 목록을 간단히 적어 보아요~~ 📝

---

👉 (이곳에 작성해주세요~)

1. CSS Diner 완료하기! (인증 이미지도 있어요~~ ✨✨)
2. 추가 예정 - 프로그래머스 알고리즘
3. 추가 예정1만시간의 법칙 과제 수행

---

<br><br>

## 오늘 학습한 내용 중 가장 기억에 남는 것들을 몇 가지 적어볼까요? 📝

---

👉 (이곳에 작성해주세요~)

어멋! 이건 꼭 외워야해!!!

```
Combine the Class Selector
A.className
class이름이 className인 A요소를 선택


#big.wide
class명이 wide이면서 id명이 big인 요소 선택




Combine the Universal Selector
A *
=> A 내부에 있는 모든 요소를 선택


p *
=> p태그 내부에 있는 모든 요소를 선택


ul.fancy *
=> ul class="fancy"요소 내에 있는 모든 요소를 선택




Adjacent Sibling Selector
p + .intro
=> <p>와 직접적으로 인접해있는 class="intro"를 가진 모든 요소를 선택

div+a
=> <div>와 직접적으로 인접한 모든 <a>태그를 선택



General Sibling Selector
A ~ B
=> A뒤에 나오는 모든 B요소를 선택



First Child Pseudo-selector
A:first-child
=> A중 첫번째 요소를 선택


p:first-child
=> <p>에 해당되는 것들 중 첫번쨰 요소를 선택


div p:first-child
=> <div>안에 있는 <p>에 해당되는 것들 중 첫번째 요소를 선택




Only Child Pseudo-selector
A:only-child
=> 부모 요소에 포함되어있는(nesting) 유일한 자식인 모든 A요소를 선택

span: only-child
=> 다른 요소의 유일한 자식인 span을 선택


ul li:only-child
=> <ul> 내에 존재하는 <li> 요소를 선택



Last Child Pseudo-selector
:last-child
=> 모든 last-child 요소를 선택


span:last-child
=> 모든 last-child <span>요소를 선택


ul li:last-child
=> 어떤 <ul>에 속하는 마지막 <li> 요소를 선택



Nth Child Pseudo-selector
:nth-child(A)
=> n번째 자식 요소를 선택

div p:nth-child(2)
=> 모든 <div>의 하위에 존재하는 <p> 중 두번째 <p> 를 선택



Nth Last Child Selector
:nth-last-child(A)
=> A 순번의 카운팅을 아래에서부터 해서 A번째에 해당하는 자식 last child element를 선택
(순번이 위에서부터가 아니다)

형제 그룹 간의 위치를 기반으로 요소를 찾는다는 점에 유의하도록 하자

아래의 예시는 1)을 선택하는 예시이다(첫번째 bento 선택)

<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Select the 1st bento</title>
    <style>
      /* 1)을 선택 */
      plate:nth-child(3) {
      }
    </style>
  </head>

  <body>
    <div class="table">
      <plate />
      <bento />
      <!-- 1) -->
      <plate>
        <orange />
        <orange />
        <orange />
      </plate>
      <bento />
    </div>
  </body>
</html>



:first-of-type
특정 타입의 첫번쨰 요소를 선택함

span:first-of-type
=> 어떤 요소 내의 첫번째 <span>태그를 선택




:nth-of-type(A)
특정한 요소를 선택 (예: 짝수, 홀수 등)할 때 사용

div:nth-of-type(2)
=> <div>의 두번쨰 인스턴스를 선택함

.example:nth-of-type(odd)
=> example 클래스의 모든 홀수 인스턴스를 선택




C:nth-of-type(An+B)
B에서 시작해서 매 A번째에 존재하는 C태그를 선택

span:nth-of-type(6n+2)
=> 2번쨰 인스턴스부터 시작해서 매 6의 배수위치에 존재하는 <span>태그를 선택




:only-of-type
동일한 타입의 형제가 없는 요소를 나타냄

p span:only-of-type
=> <p>태그 내에 존재하는 유일한 <span> 태그를 선택함
(span 태그내에 p태그가 여러개 있는 영역은 해당 사항이 없음)




A:last-of-type
모든 요소 중 마지막 A를 선택함

p span: last-of-type
=> 모든 <p>태그 내에 존재하는 <span>태그 중 마지막 <span> 태그를 선택함




A:empty
A 내부에 아무 요소도 가지지 않은 A 요소를 선택

div:empty
=> 모든 비어있는 <div>요소를 선택함




A:not(x)
x조건에 맞지 않는 A를 선택

:not(#fancy)
=> id="fancy"가 아닌 모든 요소를 선택함

div:not(:first-child)
=> first-child가 아닌 모든 <div> 태그를 선택함

:not(.big, .medium)
=> class="big" 이나 class="medium"이 아닌 모든 요소를 선택함




Attribute Selector
특정한 attribute를 가진 모든 요소를 선택

a[href]
=> href="anything" attribute를 가진 모든 <a> 요소를 선택

[type]
=> type="anything" attribute를 가진 모든 요소를 선택

예시

[for]은 ~for꼴인 요소를 선택
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Select the items for someone</title>
    <style>
      /* 누군가를 위한 아이템 3개의 공통점 - for="~"꼴 */
      [for] {
      }
    </style>
  </head>

  <body>
    <div class="table">
      <bento>
        <apple class="small" />
      </bento>
      <apple for="Ethan" />
      <plate for="Alice">
        <pickle />
      </plate>
      <bento for="Clara">
        <orange />
      </bento>
      <pickle />
    </div>
  </body>
</html>



A[attribute]
특정 attribute를 가진 모든 요소를 선택

[value]
=> value="anything" attribute를 지닌 모든 요소를 선택함

a[href]
=> href="anything" attribute를 지닌 모든 <a>요소를 선택함

input[disabled]
=> disabled attribute를 지닌 모든 <input> 요소를 선택함




Attribute Value Selector
[attribute="value"]
=> 특정 attribute value를 지니는 모든 요소를 선택

input[type="checkbox"]
=> 모든 checkbox input 요소를 선택




Attributes Starts With Selector
[attribute^="value"]
=> 특정 문자로 시작하는 모든 요소를 선택

.toy[category^="Swim"]
=> toy 클래스를 가지면서 category="Swimmer" 이거나 category="Swimming"와 같이 Swim으로 시작하는 요소들을 선택함




Attribute Ends With Selector
[attributes$="value"]
=> 특정 문자로 끝나는 모든 요소를 선택함

img[src$=".jpg"]
=> .jpg이미지를 보여주는 모든 이미지를 선택




Attribute Wildcard Selector
[attribute*="value"]
=> 특정 문자를 atrribute value로 가지는 모든 요소를 선택

class, href, src아 같은 특정 패턴을 확인할 때 유용한 선택자

img[src*="/thumbnails/"]
=> thumbnails 폴더로부터 이미지를 보여주는 모든 img 요소를 선택

class["heading"]
=> class="main-heading"이나 class="sub-heading"와 같이 "heading"을 지닌 클래스를 선택
```

---

<br><br>

## 오늘 하루 어떤 점이 가장 인상 깊었나요?? 🌛

- 2글자 이상 간단히 적어주셔도 좋아요 ⌨️ (보글보글..)
- 이미 적은 블로그 글이 있다면 링크만 걸어주셔도 좋아요 🙌🙌

---

👉 (이곳에 작성해주세요~)

<br>

css가 어렵고 까다롭다고만 느꼈는데, 간단한 게임을 통해서 빠르게 selector를 익힐 수 있어서 자신감이 한 층 올라갔어요!
- [CSS Diner 수행목록](https://github.com/kimdaeyeobbb/Web_Programming/tree/main/Study/Lectures/JCB/Homework/%5B~9.20%5D%20CSS%20Diner)

---

<br><br>

## 오늘도 꿈을 향한 우리! 혹시 공유하고 싶은 생각이 있으면 적어보아요~ 📝

---

👉 (이곳에 작성해주세요~)

저는 복습을 깃허브에 정리하면서 진행하는 편인데, 다른분들은 어떻게 진행하시는지 궁금해요!
---

<br><br>

## 우리 회고조에게 바란다 ~ 🤗

---

👉 (이곳에 작성해주세요~)


- 회고 활동에 있어 수정이 필요한 부분이 느껴진다면 얼마든지 의견을 피력해주세요!! 📝 
- 고민이 있다면 편하게 얘기해주세요! 고민은 나누면 1/2로 줄어든답니다 
- 템플릿을 깔끔하게 만들어주신 지형님께 감사의 말씀전합니다! (혹시 이러한 점은 수정했으면 좋겠다! 하는 것이 있다면 편하게 말씀해주세요)
---
