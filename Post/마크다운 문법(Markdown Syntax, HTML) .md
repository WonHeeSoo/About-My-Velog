마크다운 문법(Markdown Syntax, HTML)

| 업데이트 일자  |업데이트 내용 |
| :---:| :--- |
| 2020-02-02 |Headings 헤더가 Velog에서 사용 가능한지 여부 추가|
|  |각 주제마다 수평선 추가|
|  |목차 내용 수정|
| 2020-02-10 |벨로그 v2 업데이트에 따른 변경점 수정|
|  |벨로그 Markdown Style 변경으로 가독성 떨어지는 일부 내용 수정|
|  ||

---
# 서론

기존에 [Legacy GitBook](https://wonheesoo.gitbooks.io/study-book/content/markdown/markdown-command.html) 그리고 지금은 운영하지 않는 Hexo blog에 작성했던 내용을 옮기고 Velog에 맞게 수정하였습니다.
Velog에 작성하는 만큼 Velog에서 가능여부도 새로 추가하였습니다.

벨로그v1에서는 HTML Tag를 사용할 수 없었으나 벨로그v2부터는 HTML Tag가 사용 가능합니다.


---
# 1. Headings 헤더

| Markdown Syntax  |⬅Velog | HTML Tag | ⬅Velog | Description |
| :---| :---: | :---| :---: | :--- |
| \# 헤더1 |⭕| &lt;h1&gt;헤더1&lt;/h1&gt; |⭕| 문서의 제목(큰 제목), 글머리1(Head1) |
| \#\# 헤더2 |⭕| &lt;h2&gt;헤더2&lt;/h2&gt; |⭕| 문서의 제목(작은 제목), 글머리2(Head2) |
| \#\#\# 헤더3 |⭕| &lt;h3&gt;헤더3&lt;/h3&gt; |⭕| 글머리3(Head3) |
| \#\#\#\# 헤더4 |⭕| &lt;h4&gt;헤더4&lt;/h4&gt; |⭕| 글머리4(Head4) |
| \#\#\#\#\# 헤더5 |⭕| &lt;h5&gt;헤더5&lt;/h5&gt; |⭕| 글머리5(Head5) |
| \#\#\#\#\#\# 헤더6 |⭕| &lt;h6&gt;헤더6&lt;/h6&gt; |⭕| 글머리6(Head6) |

## ✍사용법
```
# 헤더1
```
```
## 헤더2
```
```
### 헤더3
```
```
#### 헤더4
```
```
##### 헤더5
```
```
###### 헤더6
```
```
<h1>헤더1</h1>
```
```
<h2>헤더2</h2>
```
```
<h3>헤더3</h3>   
```
```
<h4>헤더4</h4>
```
```
<h5>헤더5</h5>   
```
```
<h6>헤더6</h6>
```
## 📝결과 
# 헤더1
## 헤더2
### 헤더3
#### 헤더4
##### 헤더5
###### 헤더6
<h1>헤더1</h1>
<h2>헤더2</h2>
<h3>헤더3</h3>   
<h4>헤더4</h4>
<h5>헤더5</h5>   
<h6>헤더6</h6>

# 1-1. 그 이외 Headings 헤더
## ✍사용법
```
제목입니다.
==
```

```
부제목입니다.
--
```
## 📝결과 
제목입니다.
==
부제목입니다.
--

---

# 2. Styling text 강조구문

| Markdown Syntax |⬅Velog| HTML Tag |⬅Velog| Description |
| :--- | :---: | :---: | :---: | :--- |
| \*이탤릭체\* |⭕| &lt;em&gt;이탤릭체&lt;/em&gt; |⭕| 이탤릭체(Italic) |
| \_이탤릭체\_ |⭕| 위와 같음 | ⭕|이탤릭체(Italic) |
| \*\*볼드체\*\* |⭕| &lt;string&gt;볼드체&lt;/string&gt; |⭕ |볼드체(Bold) |
| \_\_볼드체\_\_ |⭕| 위와 같음 | ⭕|볼드체(Bold) |
|&lt;u&gt;밑줄&lt;/u&gt;|⭕|||밑줄|
|\~취소선\~|⭕|&lt;del&gt;취소선&lt;/del&gt;|⭕| 취소선 |
| \~\~취소선\~\~ ||&lt;strike&gt;취소선&lt;/strike&gt;|⭕| 취소선 |
| ^윗첨자^ |❌| &lt;sup&gt;윗첨자&lt;/sup&gt; |⭕| 윗첨자 |
|  || &lt;sub&gt;아랫첨자&lt;/sub&gt; |⭕| 아랫첨자 |
|||&lt;small&gt;작은 글씨&lt;/small&gt;|❌|작은 글씨|
|==강조==|❌|||강조(형광펜느낌)|




## ✍사용법
```
_이탤릭체_
```
```
<em>이탤릭체</em>
```
```
**볼드체**
```
```
<string>볼드체</string>
```
```
<u>밑줄</u>
```
```
~~취소선~~
```
```
<del>취소선</del>
```
```
<strike>취소선</strike>
```
```
윗첨자^윗첨자^
```
```
윗첨자<sup>윗첨자</sup>
```
```
아랫첨자<sub>아랫첨자</sub>
```
```
==강조==
```
## 📝결과

_이탤릭체_
<em>이탤릭체</em>
**볼드체**
<string>볼드체</string>
<u>밑줄</u>
~~취소선~~
<del>취소선</del>
<strike>취소선</strike>
윗첨자^윗첨자^
아랫첨자<sup>윗첨자</sup>
아랫첨자<sub>아랫첨자</sub>
==강조==
>### 💡 기본적인 마크다운 문법을 기반으로 다양하게 변형된 마크다운 문법이 많습니다.

# 2-2. 강제 개행과 그 이외
| HTML Tag |⬅Velog| Description |
| :---: | :---: | :--- |
|`<br>`|⭕|강제 개행|
|`&nbsp;`|⭕|강제 개행(Non-breaking Space)|
|`&#32;`|⭕|강제 개행|
    

> ### 💡 `&#32;`과 `&nbsp;`는 Tag 보다는 HTML에서 사용되는 특수문자 기호에 가깝습니다.

> ### 💡 강제 개행 뿐만 아니라 &amp;, &gt;, &euro; , &micro; 등등 다양한 기호가 존재하며 Velog에서 사용 가능합니다.
> ### [HTML Characters and Symbols](https://ascii.cl/htmlcodes.htm)


---
# 3. Quoting code, Fenced code blocks 인라인 코드, 코드 블럭

| Markdown Syntax | ⬅Velog | HTML Tag | ⬅Velog | Description |
| :--- | :---: | :---  | :---: | :--- |
| \`Mark인용코드1\` |⭕| &lt;code&gt;Tag인용 코드1&lt;/code&gt; |⭕| 인용 코드1 |
| \`\`\`Mark인용코드2\`\`\` |⭕| &lt;pre&gt;Tag인용 코드2&lt;/pre&gt; |⭕| 인용 코드2 |
| 위와 같음 || &lt;pre&gt;&lt;code&gt;Tag인용 코드3&lt;/code&gt;&lt;/pre&gt; |⭕| 인용 코드3 |

## ✍사용법
```
`Mark인용코드1`
```
```
<code>Tag인용 코드1</code>
```

```
```HTML
<!DOCTYPE html>
<html>
<head>
<title>Page Title</title>
</head>
<body>
``````

```
```CSS
int main()
{
  cout << "Hello World!" << endl;
}
``````
```
<pre>Tag인용 코드2</pre>
```
```
<pre><code>Tag인용 코드3</code></pre>
```
```
   Tab을 누르고 입력하면 자동으로 코드블럭이 생성됩니다.
```
## 📝결과
`Mark인용 코드1`

<code>Tag인용 코드1</code>

```HTML
<!DOCTYPE html>
<html>
<head>
<title>Page Title</title>
</head>
<body>

```

```CSS
int main()
{
  cout << "Hello World!" << endl;
}
```

<pre>Tag인용 코드2</pre>

<pre><code>Tag인용 코드3</code></pre>

   Tab을 누르고 입력하면 자동으로 코드블럭이 생성됩니다.

> ### 💡 다양한 언어의 하이라이팅을 지원합니다. (괄호안의 단어로 사용)
> - Bash (bash)
- C# (cs)
- C++ (cpp)
- CSS (css)
- Diff (diff)
- HTML, XML (html)
- HTTP (http)
- Ini (ini)
- JSON (json)
- Java (java)
- JavaScript (javascript)
- PHP (php)
- Perl (perl)
- Python (python)
- Ruby (ruby)
- SQL (sql)

> ### 💡 코드블럭에 사용되는 `(억음부호, backtick)는 보통 키보드 Tab위에 있습니다.

---

# 4. Quoting text 인용구

| Markdown Syntax | ⬅Velog| HTML Tag | ⬅Velog| Description |
| :--- | :--: | :--- | :--:  | :--- |
| \> 인용구 |⭕|  &lt;Blockquote&gt;인용구&lt;/Blockquote&gt; |⭕| 인용구 |

## ✍사용법

```
> # 제목
> 인용구
```

```
<Blockquote>
인용구 내용
</Blockquote>
```
## 📝결과

> # 제목
> 인용구

<Blockquote>
인용구 내용
</Blockquote>

> ### 💡 인용구는 이중, 삼중 이상으로 사용 가능합니다.
> > 두 개
>>> 세 개

> ### 💡 인용구는 한번만 사용하면 라인마다 `>`(인용구)를 입력할 필요가 없습니다.
## ✍사용법
```
> 인용구
하나
둘
셋
넷
```

## 📝결과
> 인용구
하나
둘
셋
넷

---

# 5. Links 링크

## ✍사용법

```
[Velog](https://velog.io/)
```
```HTML
<a href="https://velog.io/">링크걸기</a>
```
```
https://velog.io/@wonhs717
```
```
[Youtube](https://www.youtube.com/?hl=ko&gl=KR "이것은 하이퍼링크의 설명을 작성할 수 있습니다.")
```
```
[My Velog][My link]

[My link]: https://velog.io/@wonhs717
```
```
❌ Velog에서 사용 불가 
텍스트 작성 중간에 [Link]를 사용할 수 있습니다.

[Link] : https://github.com/WonHeeSoo "저의 Github입니다"
```
## 📝결과
[Velog](https://velog.io/)
<a href="https://velog.io/">링크걸기</a>
https://velog.io/
[Youtube](https://www.youtube.com/?hl=ko&gl=KR "이것은 하이퍼링크의 설명을 작성할 수 있습니다.")
[My Velog][My link]

[My link]: https://velog.io/@wonhs717

---

# 6. Lists 리스트

| Markdown Syntax | ⬅Velog | HTML Tag | ⬅Velog | Description |
| :--- | :---: | :--- | :---:| :--- |
| \- 리스트1 |⭕| &lt;ul&gt;&lt;li&gt;리스트1&lt;/li&gt;&lt;/ul&gt; |⭕| 목록(unordered list) |
| \* 리스트2 |⭕| 위와 같음 || 목록(unordered list) |
| \+ 리스트3 |⭕| 위와 같음 || 목록(unordered list) |
| 1\. 리스트4 |⭕| &lt;ol&gt;&lt;li&gt;리스트4&lt;/li&gt;&lt;/ol&gt; |⭕| 목록(ordered list) |

## ✍사용법

```
- 리스트1
* 리스트2
+ 리스트3
1. 리스트4
```
```
<ol>
  <li>리스트4-1</li>
  <li>리스트4-2</li>
</ol>
```
```
<ul>
  <li>리스트1-1</li>
  <li>리스트1-1</li>
  <li>리스트1-1</li>
    <ol>
      <li>리스트4-3</li>
      <li>리스트4-4</li>
    </ol>
</ul>
```

## 📝결과

- 리스트1
* 리스트2
+ 리스트3
1. 리스트4

<ol>
  <li>리스트4-1</li>
  <li>리스트4-2</li>
</ol>

<ul>
	<li>리스트1-1</li>
	<li>리스트1-1</li>
	<li>리스트1-1</li>
	  <ol>
		  <li>리스트4-3</li>
		  <li>리스트4-4</li>
		</ol>
</ul>


# 6-1. 그 이외 Lists 리스트

리스트를 만든 상태에서 바로 아래에 탭(Tab) 한번 혹은 스페이스(Space) 두 번 정도의 공백을 한 뒤 리스트(\-)를 사용하면 기존 리스트의 하위 리스트를 만들수 있습니다.

## ✍사용법

```
- A리스트1
	- A리스트2
    	- A리스트3
```
```
- B리스트1
  * B리스트2
    1. B리스트3
```

## 📝결과

- A리스트1
	- A리스트2
    - A리스트3


- B리스트1
  * B리스트2
  1. B리스트3

---

# 7. Task lists 할일 리스트, 체크 리스트

| Markdown Syntax | ⬅Velog| HTML Tag | Description |
| :--- | :---: | :--- | :--- |
| \- \[ ] |⭕| | 체크박스\(false\) |
| \- \[x] |⭕| | 체크박스\(true\) |

## ✍사용법

```
- [ ] 체크박스(false)
- [x] 체크박스(true)
```

## 📝결과

- [ ] 체크박스(false)


- [x] 체크박스(true)

---

# 8. Table 테이블

## ✍사용법

```
| 제목1 | 제목2 | 제목3 | 제목4 |
| :- | - | :-: | -: |
| 내용1입니다 | 내용2입니다 | 내용3입니다 | 내용4입니다 |
| 내용1 | 내용2 | 내용3 | 내용4 |
```
```
| <center>제목1</center> | 제목2 | 제목3 | <center>제목1</center> |
| :- | - | :-: | -: |
| 내용1입니다 | 내용2입니다 | 내용3입니다 | 내용4입니다 |
| 내용1 | 내용2 | 내용3 | 내용4 |
```
## 📝결과

| 제목1 | 제목2 | 제목3 | 제목4 |
| :- | - | :-: | -: |
| 내용1입니다 | 내용2입니다 | 내용3입니다 | 내용4입니다 |
| 내용1 | 내용2 | 내용3 | 내용4 |

| <center>제목1</center> | 제목2 | 제목3 | <center>제목1</center> |
| :- | - | :-: | -: |
| 내용1입니다 | 내용2입니다 | 내용3입니다 | 내용4입니다 |
| 내용1 | 내용2 | 내용3 | 내용4 |

# 8-1. 그 이외 Table 사용법

> ### 💡 표를 사용할때 `-`의 수는 상관없습니다.
## ✍사용법
```
| 제목1 | 제목2 | 제목3 | 제목4 |
| :---- | ------ | :----------: | --------------------: |
| 내용1입니다 | 내용2입니다 | 내용3입니다 | 내용4입니다 |
| 내용1 | 내용2 | 내용3 | 내용4 |
```
## 📝결과
| 제목1 | 제목2 | 제목3 | 제목4 |
| :---- | ------ | :----------: | --------------------: |
| 내용1입니다 | 내용2입니다 | 내용3입니다 | 내용4입니다 |
| 내용1 | 내용2 | 내용3 | 내용4 |

<br>

> ### 💡 두번째 줄의 `:--:`, `----`, `----`같은 표현은 표의 정렬 기준입니다.
`---` 정렬하지 않음
`:---` 왼쪽으로 정렬
`---:` 오른쪽으로 정렬
`:---:` 가운데 정렬
## ✍사용법
```
| 제목1 | 제목2 | 제목3 | 제목4 |
| --- | :--- | :---: | ---: |
| 이곳은 | 여기는 | 가운데 | 왼쪽 |
| 정렬을 사용하지 않는 | 오른쪽 | 정렬을 사용 | 정렬을 |
| 공간 | 정렬을 하는 곳 | 하는 곳 | 하는 곳입니다 |
```
## 📝결과
| 제목1 | 제목2 | 제목3 | 제목4 |
| --- | :--- | :---: | ---: |
| 이곳은 | 여기는 | 가운데 | 왼쪽 |
| 정렬을 사용하지 않는 | 오른쪽 | 정렬을 사용 | 정렬을 |
| 공간 | 정렬을 하는 곳 | 하는 곳 | 하는 곳입니다 |

<br>

> ### 💡 특정 방향으로 정렬해도 HTML Tag인 `<center></center>`를 사용하면 가운데 정렬이 되지만 Velog에서는 사용할 수 없습니다. 
## ✍사용법
```
| <center>제목1</center> |  <center>제목2</center> |
| :- |  -: |
| <center>내용1입니다</center> | <center>내용2입니다</center> |
| 내용1 | 내용2|
| <center>내용1</center> | <center>내용2</center> |
```
## 📝결과
| <center>제목1</center> |  <center>제목2</center> |
| :- |  -: |
| <center>내용1입니다</center> | <center>내용2입니다</center> |
| 내용1 | 내용2|
| <center>내용1</center> | <center>내용2</center> |

---

# 9. Horizontal Rules 수평선

| Markdown Syntax | ⬅Velog | HTML Tag| ⬅Velog | Description |
| :--- | :---: | :--- | :---: | :--- |
| \-\-\- |⭕| &lt;hr/&gt; |⭕| 수평선 |
| \*\*\* |⭕|  || 수평선 |
| \_\_\_ |⭕|  || 수평선 |
| \* \* \* |⭕|  || 수평선 |
| \- \- \- |⭕|  || 수평선 |

## ✍사용법
```
---
```
```
***
```
```
___
```
```
* * *
```
```
- - -
```
```
<hr/>
```

## 📝결과

---
***
___
* * *
- - -
<hr/>

---

# 10. Backslash escapes

| Markdown Syntax | ⬅Velog| Description |
| :--- | :---:| :--- |
| \\\\ |⭕| backslash |
| \\\` |⭕| backtick |
| \\\* |⭕| asterisk |
| \\\_ |⭕| underscore |
| \\\{ |⭕| curly braces |
| \\\} |⭕| curly braces |
| \\\[ |⭕| square brackets |
| \\\] |⭕| square brackets |
| \\\( |⭕| parentheses |
| \\\) |⭕| parentheses |
| \\\# |⭕| hash mark |
| \\\+ |⭕| plus sign |
| \\\- |⭕| minus sign (hyphen) |
| \\\. |⭕| dot |
| \\\! |⭕| exclamation mark |

## ✍사용법
```
\\
```
```
\`
```
```
\*
```
```
\_
```
```
\{ \}
```
```
\[ \]
```
```
\( \)
```
```
\#
```
```
\+
```
```
\-
```
```
\.
```
```
\!
```
## 📝결과
\\

\`

\*

\_

\{ \}

\[ \]

\( \)

\#

\+

\-

\.

\!


---

# 11. Emoji 이모지
## 첫번째 방법 : 단축키
**Windows 10 단축키**
`윈도우키` + `.`
`윈도우키` + `;`

**Mac 단축키**
`Ctrl` + `Command` + `스페이스 바`
[Mac에서 이모티콘, 강세 표시 및 기호를 사용하는 방법](https://support.apple.com/ko-kr/HT201586)
## 두번째 방법 : Copy & Paste 복사 붙여넣기
[Emojipedia](https://emojipedia.org/) : 카테고리 혹은 검색해서 Emoji를 찾을 수 있는 페이지
[GetEmoji](https://getemoji.com/) : Emojipedia의 Emoji들을 바로 복사할 수 있도록 만든 페이지

## 세번째 방법 : Windows 10 터치 키보드

![First](https://github.com/WonHeeSoo/About-My-Velog/blob/master/Images/Window10Emoji/01LowBarMouseRightButtonClick.PNG?raw=true)
**작업 표시줄(하단 아이콘 바)**를 마우스 오른쪽 클릭하여 **터치 키보드 단추 표시(Y)**를 선택합니다.

![First](https://github.com/WonHeeSoo/About-My-Velog/blob/master/Images/Window10Emoji/02TouchKeyboardClick.PNG?raw=true)
**작업 표시줄(하단 아이콘 바)** 오른쪽에 키보드 모양의 **터치 키보드 아이콘**을 선택합니다.


![First](https://github.com/WonHeeSoo/About-My-Velog/blob/master/Images/Window10Emoji/03SmileButtonClick.PNG?raw=true)
터치 키보드 왼쪽 하단에 **이모티콘 아이콘**을 선택합니다.

![First](https://github.com/WonHeeSoo/About-My-Velog/blob/master/Images/Window10Emoji/04EmojiClick.PNG?raw=true)
원하는 아이콘을 선택합니다.

---

# 12. Image 이미지
| Markdown Syntax | ⬅Velog| HTML Tag | ⬅Velog| Description |
| :---  | :---: | :--- | :---: | :--- |
| \!\[제목]\(주소, 확장자명) |⭕| &lt;img alt\=\"제목\" src\=\"주소, 확장자명\" \/&gt; |❌| 이미지 출력 |

## ✍사용법

```
![제목](주소)
```
```
![ImageExample](https://github.com/WonHeeSoo/GitBook_StudyBook/blob/master/image/Image%20Example.PNG?raw=true)
```
```
<img alt="ImageExample" src="https://github.com/WonHeeSoo/GitBook_StudyBook/blob/master/image/Image%20Example.PNG?raw=true" />
```

## 📝결과
![제목](주소)
![ImageExample](https://github.com/WonHeeSoo/GitBook_StudyBook/blob/master/image/Image%20Example.PNG?raw=true)
<img alt="ImageExample" src="https://github.com/WonHeeSoo/GitBook_StudyBook/blob/master/image/Image%20Example.PNG?raw=true" />

---

# 13. Video

> ### 💡 Velog에서는 하이퍼링크가 있는 이미지라고 생각하시면 됩니다.

Markdwon은 기본적으로 동영상을 지원하지 않으나 도구에 따라 마크다운 문법이 확장되어 단순히 주소만 복사해줘도 동영상을 올리는 것이 가능하지 않을 때 사용합니다.

최소한의 코드는 다음과 같습니다.
`[![영상 제목](이미지주소)](영상주소)`

일종의 트릭으로 Markdwon의 Link(`[링크제목](링크주소)`)와 Image(`![제목](주소)`)를 사용하여 Image자체를 링크의 제목으로 만들고 링크주소를 걸어주면 됩니다.

# 13-1. Youtube

### Youtube Thumbnail을 사용하는 방법

[![BTS DNA Youtube](https://img.youtube.com/vi/MBdVXkSdhwU/0.jpg)](https://www.youtube.com/watch?v=MBdVXkSdhwU)
`
[![BTS DNA Youtube](https://img.youtube.com/vi/MBdVXkSdhwU/0.jpg)](https://www.youtube.com/watch?v=MBdVXkSdhwU)
`

위의 코드 중에서 이미지 주소인 `https://img.youtube.com/vi/MBdVXkSdhwU/0.jpg)`, 특히 끝부분을 보면 `MBdVXkSdhwU/0`라는 부분이 있는데 영상의 링크 주소를 확인해보면 `MBdVXkSdhwU`이 존재함을 알 수 있고 동영상의 고유 주소임을 알 수 있습니다.

여기서 추가적으로 `/0`부분이 의미하는 것은 고유의 코드로 영상 게시자가 선택한 Thumbnail을 우리가 사용할 수 있습니다.

또한 `/0` 대신 `/1`, `/2`, `/3`, `/default`, `/mqdefault`, `/hqdefault`, `/dsdefault`, `/maxresdefault`을 사용할 수 있습니다.

#### `/1`을 사용한 예

[![BTS DNA Youtube/1](https://img.youtube.com/vi/MBdVXkSdhwU/1.jpg)](https://www.youtube.com/watch?v=MBdVXkSdhwU)

#### `/2`을 사용한 예

[![BTS DNA Youtube/2](https://img.youtube.com/vi/MBdVXkSdhwU/2.jpg)](https://www.youtube.com/watch?v=MBdVXkSdhwU)

#### `/3`을 사용한 예

[![BTS DNA Youtube/3](https://img.youtube.com/vi/MBdVXkSdhwU/3.jpg)](https://www.youtube.com/watch?v=MBdVXkSdhwU)

#### `/default`을 사용한 예

[![BTS DNA Youtube/default](https://img.youtube.com/vi/MBdVXkSdhwU/default.jpg)](https://www.youtube.com/watch?v=MBdVXkSdhwU)

#### `/mqdefault`을 사용한 예

[![BTS DNA Youtube/mqdefault](https://img.youtube.com/vi/MBdVXkSdhwU/mqdefault.jpg)](https://www.youtube.com/watch?v=MBdVXkSdhwU)

#### `/hqdefault`을 사용한 예

[![BTS DNA Youtube/hqdefault](https://img.youtube.com/vi/MBdVXkSdhwU/hqdefault.jpg)](https://www.youtube.com/watch?v=MBdVXkSdhwU)

#### `/sddefault`을 사용한 예

[![BTS DNA Youtube/sddefault](https://img.youtube.com/vi/MBdVXkSdhwU/sddefault.jpg)](https://www.youtube.com/watch?v=MBdVXkSdhwU)

#### `/maxresdefault`을 사용한 예

[![BTS DNA Youtube/sddefault](https://img.youtube.com/vi/MBdVXkSdhwU/maxresdefault.jpg)](https://www.youtube.com/watch?v=MBdVXkSdhwU)

### Youtube Video Thumbnail을 사용하는 방법
> ### 💡 Video Thumbnail 주소가 변경 가능성이 있어 이 방법은 보류

[![BTS DNA Youtube](https://i.ytimg.com/an_webp/MBdVXkSdhwU/mqdefault_6s.webp?du=3000&sqp=CJmTg9MF&rs=AOn4CLDAp7iix1IMI4mn2VTQzd5SBz9lmA)](https://www.youtube.com/watch?v=MBdVXkSdhwU)
`[![BTS DNA Youtube](https://i.ytimg.com/an_webp/MBdVXkSdhwU/mqdefault_6s.webp?du=3000&sqp=CJmTg9MF&rs=AOn4CLDAp7iix1IMI4mn2VTQzd5SBz9lmA)](https://www.youtube.com/watch?v=MBdVXkSdhwU)`

원하는 영상을 검색한뒤 Youtube Video Thumbnail이 작동하는 영상을 마우스 우클릭을 해 이미지 주소 복사를 합니다.

![Youtube Video Thumbnail Mobile](/images/PostImages/Markdown1/YoutubeVideoThumbnailMobileImage.png)

모바일의 경우 Video Thumbnail이 보이지 않습니다.

### Youtube 특정 시간대 영상 재생하기

[![Everything Is AWESOME](https://img.youtube.com/vi/MBdVXkSdhwU/0.jpg)](https://youtu.be/MBdVXkSdhwU?t=29)
`[![Everything Is AWESOME](https://img.youtube.com/vi/MBdVXkSdhwU/0.jpg)](https://youtu.be/MBdVXkSdhwU?t=29)`

Thumbnail의 크기나 이미지를 선택하기 위해 각 영상들만의 고유코드 뒤에 `/0`이나 `/default`같은 것을 붙였고 시간의 경우 고유코드 뒤에 `/?t=원하는시간`을 적으면 특정 시간대에서 부터 영상을 재생시킬 수 있으며 `?t=10`은 영상의 10초 구간이며 default 값은 초(Seconds)로 계산합니다.

예를 들어 단순히 숫자 10를 적으면 영상의 10초(Seconds)에 해당하는 구간으로 이동하지만 `/?t=10m`이면 영상의 10분에 해당하는 구간, `/?t=10h`이면 영상의 10시간에 해당하는 구간부터 영상을 재생시킬 수 있습니다.

`/?t=1m24s`같이 시,분,초를 섞을 수 있습니다.

만약 영상의 길이보다 긴 시간을 적는 다면 영상의 끝 부분으로 이동해 영상이 끝나거나 다시 영상의 첫 부분부터 다시 재생이 됩니다.

### HTML Tag을 사용하는 방법

#### HTML Tag를 사용하기

<div align="center"> <a href="https://www.youtube.com/watch?v=MBdVXkSdhwU
" target="_blank"><img src="https://img.youtube.com/vi/MBdVXkSdhwU/0.jpg"
alt="BTS DNA Youtube" width="500" height="360" border="4" /></a></div>
```
<div align="center">
  <a href="https://www.youtube.com/watch?v=MBdVXkSdhwU
" target="_blank"><img src="https://img.youtube.com/vi/MBdVXkSdhwU/0.jpg"
alt="BTS DNA Youtube" width="500" height="360" border="4" /></a>
</div>
```

#### 최소한의 HTML Tag만 사용하기

<a href="https://www.youtube.com/watch?v=MBdVXkSdhwU">
<img src="https://img.youtube.com/vi/MBdVXkSdhwU/0.jpg" ></a>
```
<a href="https://www.youtube.com/watch?v=MBdVXkSdhwU">
<img src="https://img.youtube.com/vi/MBdVXkSdhwU/0.jpg" ></a>
```


#### 최소한의 HTML Tag만 사용하기 + 제목

<a href="https://www.youtube.com/watch?v=MBdVXkSdhwU">
<img src="https://img.youtube.com/vi/MBdVXkSdhwU/0.jpg"
alt="BTS DNA Youtube"></a>
```
<a href="https://www.youtube.com/watch?v=MBdVXkSdhwU">
<img src="https://img.youtube.com/vi/MBdVXkSdhwU/0.jpg"
alt="BTS DNA Youtube"></a>
```

# 13-2. vimeo

### Vimeo Thumbnail을 사용하는 방법

[![Young Marco](https://i.vimeocdn.com/video/625196300_560x290.jpg)](https://vimeo.com/209607366)
`[![Young Marco](https://i.vimeocdn.com/video/625196300_560x290.jpg)](https://vimeo.com/209607366)`

동영상 이미지의 경우 오른쪽 하단에 위치한 다음 동영상 자동 재생에서 이미지 주소 복사를 하거나 따로 이미지를 구해서 주소 복사를 합니다.

Vimeo의 경우 이미지 주소 뒤에 `_가로x세로.jpg`를 붙이면 원하는 크기로 출력됩니다.

### Vimeo 특정 시간대 영상 재생하기

[![Young Marco](https://i.vimeocdn.com/video/625196300_560x290.jpg)](https://vimeo.com/209607366#t=30s)
`[![Young Marco](https://i.vimeocdn.com/video/625196300_560x290.jpg)](https://vimeo.com/209607366#t=30s)`

Vimeo는 영상 주소 뒤에 `#t=시간`을 붙이면 됩니다. Youtube와 마찬가지로 default값은 초(Seconds)이며 `m`, `h`를 사용할 수 있으며 Youtube처럼 `#t=1m20s` 이런 식으로 섞을 수 있습니다.

만약 영상의 길이보다 긴 시간을 적는 다면 영상의 끝 부분으로 이동해 영상이 끝납니다.

### 다른 동영상 플레이어의 경우

그에 맞는 API를 사용하거나 없다면 단순히 링크 주소만 사용합니다.

---

# 14. 목차
> ### ❌ Velog에서 사용 불가

Velog를 포함하여 적용 안되는 곳이 많습니다.
Velog에서 자동으로 헤더를 읽어서 오른쪽에 표시 했으니 그것을 사용하면 될 것 같습니다.

## ✍사용법
`[TOC]`, `[toc]`

---

# 15. Footnotes 각주

> ### ❌ Velog에서 사용 불가

| Markdown Syntax |HTML Tag | Description |
| :--- |:--- | :--- |
| \[^1\] || 각주 |

## ✍사용법

```
Velog[^1]는 Velog입니다.
[^1]:Velig는 블로그 프레임워크입니다.
```
## 📝결과

Velog[^1]는 Velog입니다.

[^1]:Velog는 블로그입니다.

---

# 16. Username @mentions \( GitHub Flavored Markdown \)

> ### ❌ Velog에서 사용 불가

`@유저닉네임`을 사용하면 그 유저닉네임을 가진 사람에게 댓글을 보도록 알릴 수 있습니다.

혹은 조직 내의 팀에게도 사용 가능합니다.

#### 원문
> Typing an @ symbol, followed by a username, will
notify that person to come and view the comment\.
This is called an “@mention”, because you’re
mentioning the individual\. You can also @mention
teams within an organization\.

---

# 17. Using emoji \( GitHub Flavored Markdown \)

> ### ❌ Velog에서 사용 불가

| Markdown Syntax | Description |
| :--- | :--- |
| `:+1:` | +1 |
| `:sparkles:` | sparkles |
| `:camel:` | camel |
| `:tada:` | tada |
| `:rocket:` | rocket |
| `:metal:` | metal |
| `:octocat:` | octocat |

:+1: :sparkles: :camel: :tada:
:rocket: :metal: :octocat:

#### 추가적인 Emoji

[EMOJI CHEAT SHEET](https://www.webpagefx.com/tools/emoji-cheat-sheet/)