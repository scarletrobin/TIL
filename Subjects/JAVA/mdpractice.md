# 마크다운의 장점
1. 문법이 쉽다.
2. 관리가 쉽다.
3. 지원 가능한 플랫폼과 프로그램이 다양하다.

# 마크다운의 단점
1. 표준이 없어 사용자마다 문법이 상이할 수 있다.
2. 모든 HTML 마크업을 대신하지 못한다.

# 마크다운 문법

## 제목 (Header)

# 제목 1
## 제목 2
### 제목 3
#### 제목 4
##### 제목 5
###### 제목 6  
<br>

  
## 강조(Emphasis)

이탤릭체는 `*별표*` 혹은 `_언더바_` 를 사용하세요.<br>
   _안녕하세요_  
   *반갑습니다*  
   취소선은 `~~물결표시~~`를 사용하세요.
     
  ~~취소선입니다.~~  
   밑줄은 `<u>밑줄태그</u>`를 사용하세요.

  <u>밑줄입니다.</u>
<br>  


## 목록 (List)

1. 순서가 필요한 목록?
2. 이렇게 번호를 적고 띄어쓰기하면 끝!
3. 참 쉽죠?

순서가 필요없는 목록은
`-대쉬`, `*별표`, `+더하기` 중 하나를 택하면 된답니다.
* 안녕하세요
* 반갑습니다.
* 바로 자동으로 입력이 되네요. 신기?
  
<br>

## 링크 (Links)
```[Google](https://google.com) 
[Naver](https://naver.com "링크설명(title)을 작성하세요.")
```
문서 안에서 [참조 링크]를 그대로 사용할 수도 있습니다.

다음과 같이 문서 내 일반 url이나 꺾쇠 괄호 (angle brackets)안의 url은 자동으로 링크를 사용합니다.

구글 홈페이지: https://google.com
네이버 홈페이지: <https://naver.com>

[Dribble link]: https://dribble.com

[1]: https://github.com
[참조 링크]: https://naver.com "네이버로 이동합니다"

<br>

## 이미지 (Image)
링크와 비슷하지만 앞에 !가 붙습니다.
![대체 텍스트(alternative text)를 입력하세요!](https://www.gstatic.com/webp/gallery/5.jpsg "링크 설명(title)을 작성하세요")

![Kayak][logo]

[logo]: http://www.gstatic.com/webp/gallery/2.jpg "To go kayaking."

## 이미지에 링크
마크다운 이미지 코드를 링크 코드로 묶어 줍니다.

[![Vue](/images/vue.png)](https://kr.vuejs.org/)

<br>

## 코드 강조

숫자 1번 키 왼쪽에 있는 `grave`를 입력하세요. (양 옆으로)

`안녕하세요`  
`코드를 강조할 때 사용`

### 인라인 코드 강조

background 혹은 background-image 속성으로 요소에 배경 이미지를 삽입할 수 있습니다.

### 블록 코드 강조 

`를 3번 이상 입력하고 코드 종류도 적습니다.

```html
<a href="https://www.google.co.kr/" target="_blank">GOOGLE</a>
```

```css
.list>li{
    position: absolute;
    top: 40px;
}
```

```javascript
function func(){
    var a = 'AAA';
    return a;
}
```

<br>

## 표 (Table)

헤더 셀을 구분할 때 3개 이상의 `-(hyphen/dash)`기호가 필요합니다. 헤더 셀을 구분하면서 `:(colons)` 기호로 셀(열/칸) 안에 내용을 정렬할 수 있습니다.
가장 좌측과 가장 우측에 있는 `|(vertical bar)` 기호는 생략 가능합니다.

```
값 | 의미 | 기본값
---|:---:|---:
`static`|유형(기준)없음/배치 불가능 | `static`
`relative`|요소 **자신**을 기준으로 배치 | 
`absolute` | 위치상 **_부모_(조상)요소**를 기준으로 배치 |
`fixed`|**브라우저창**을 기준으로 배치 | 

```


값 | 의미 | 기본값
---|:---:|---:
`static`|유형(기준)없음/배치 불가능 | `static`
`relative`|요소 **자신**을 기준으로 배치 | 
`absolute` | 위치상 **_부모_(조상)요소**를 기준으로 배치 |
`fixed`|**브라우저창**을 기준으로 배치 | 


## 인용문(Blockquote)

`<blockquote>` 태그로 변환됩니다.

<blockquote>
인용문(blockquote)<br>
>남의 말이나 글에서 직접 또는 간접으로 따온 문장.

BREAK!

>인용문을 작성하세요!
>>중첩된 인용문을 사용할 수 있습니다.
>>> 중중첩된 인용문 1 <br>
>>> 중중첩된 인용문 2 <br>
>>> 중중첩된 인용문 3 <br>
</blockquote>

## 원시 HTML (Raw Html)

마크다운 문법이 아닌 원시 html 문법을 사용할 수 있습니다.

```html
<u>마크다운에서 지원하지 않는 기능</u>를 사용할 때 유용하며 대부분 잘 동작합니다.
```

## 수평선(Horizontal Rule)
각 기호를 3개 이상 입력하세요.

```
---(hyphens)
***(asterisks)
___(underscores)
```

---

***

___
 
다 똑같은 수평선으로 작동합니다.

## 줄바꿈 (Line breaks)

```
동해물과 백두산이 마르고 닳도록  
하느님이 보우하사 우리나라 만세 <!--띄어쓰기 2번-->  
무궁화 삼천리 화려 강산<br>
대한 사람 대한으로 길이 보전하세
```

일반 줄바꿈이 동작하지 않는 환경(설정 및 버전에 따라)의 경우, '2번의 띄어쓰기'나 `<br>`를 활용할 수 있습니다.


<blockquote>본 내용은 
https://heropy.blog/2017/09/30/markdown/
에서 가져온 내용입니다. 감사합니다.
</blockquote>