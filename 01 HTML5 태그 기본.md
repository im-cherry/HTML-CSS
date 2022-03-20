# 01 HTML5 태그 기본

> 목차
>
> 1. [HTML5 페이지 구조](#1-html5-페이지-구조)
> 2. [글자 태그](#2-글자-태그)
> 3. [목록 태그](#3-목록-태그)
> 4. [테이블 태그](#4-테이블-태그)
> 5. [이미지 태그](#5-이미지-태그)
> 6. [오디오 태그](#6-오디오-태그)
> 7. [비디오 태그](#7-비디오-태그)
> 8. [입력 양식 태그](#8-입력-양식-태그)
> 9. [공간 분할 태그](#9-공간-분할-태그)

### 1. HTML5 페이지 구조

#### 기본적인 HTML5 페이지

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />
    <title>HTML5 Basic Page</title>
    <script src="script.js"></script>
    <link rel="stylesheet" type="text/css" href="style.css" />
    <style>
      body {
        background-color: yellow;
      }
    </style>
  </head>
  <body></body>
</html>
```

| head 태그 내부에 넣을 수 있는 태그 | 설명                                 |
| :--------------------------------: | :----------------------------------- |
|                meta                | 웹 페이지에 추가 정보를 전달합니다.  |
|               title                | 웹 페이지의 제목                     |
|               script               | 웹 페이지에 스크립트를 추가합니다.   |
|                link                | 웹 페이지에 다른 파일을 추가합니다.  |
|               style                | 웹 페이지에 스타일시트를 추가합니다. |

### 2. 글자 태그

| 태그 이름 | 설명                                                            |
| :-------: | :-------------------------------------------------------------- |
|    h1     | 첫 번째로 큰 제목 글자 태그                                     |
|    h2     | 두 번째로 큰 제목 글자 태그                                     |
|    h3     | 세 번째로 큰 제목 글자 태그                                     |
|    h4     | 네 번째로 큰 제목 글자 태그                                     |
|    h5     | 다섯 번째로 큰 제목 글자 태그                                   |
|    h6     | 여섯 번째로 큰 제목 글자 태그                                   |
|     p     | 본문 글자 태그                                                  |
|    br     | 줄바꿈 태그                                                     |
|    hr     | 수평 줄 태그                                                    |
|     a     | 앵커 태그 (href 속성을 사용하여 이동하고자 하는 웹 페이지 지정) |
|     b     | 굵은 글자 태그                                                  |
|     i     | 기울어진 글자 태그                                              |
|   small   | 작은 글자 태그                                                  |
|    sub    | 아래에 달라 붙는 글자 태그                                      |
|    sup    | 위에 달라 붙는 글자 태그                                        |
|    ins    | 밑줄 글자 태그                                                  |
|    del    | 가운데 줄이 그어진 글자 태그                                    |

### 3. 목록 태그

| 태그 이름 | 설명                  |
| :-------: | :-------------------- |
|    ul     | 순서가 없는 목록 태그 |
|    ol     | 순서가 있는 목록 태그 |
|    li     | 목록 요소             |
|    dl     | 정의 목록 태그        |
|    dt     | 정의 용어 태그        |
|    dd     | 정의 설명 태그        |

### 4. 테이블 태그

```html
<body>
  <table border="1">
    <tr>
      <th colspan="3">Table Data</th>
      <th rowspan="3">Table Data</th>
    </tr>
    <tr>
      <td>Table Data</td>
      <td rowspan="2">Table Data</td>
      <td>Table Data</td>
    </tr>
    <tr>
      <td>Table Data</td>
      <td>Table Data</td>
    </tr>
  </table>
</body>
```

| 태그 이름 | 설명                   |
| :-------: | :--------------------- |
|   table   | 표 태그                |
|    tr     | 표 내부의 행 태그      |
|    th     | 행 내부의 제복 셀 태그 |
|    td     | 행 내부의 일반 셀 태그 |

| 태그 이름 | 속성 이름 | 설명                    |
| :-------: | :-------: | :---------------------- |
|   table   |  border   | 표의 테두리 두께를 지정 |
|  th, td   |  rowspan  | 셀의 높이 지정          |
|           |  colspan  | 셀의 너비 지정          |

### 5. 이미지 태그

```html
<body>
  <img src="Penguins.jpg" alt="펭귄" width="300" />
</body>
```

| 속성 이름 | 설명                              |
| :-------: | :-------------------------------- |
|    src    | 이미지의 경로 지정                |
|    alt    | 이미지가 없을 때 나오는 글자 지정 |
|   width   | 이미지의 너비 지정                |
|  height   | 이미지의 높이 지정                |

### 6. 오디오 태그

```html
<body>
  <audio
    src="Kalimba.mp3"
    preload="auto|metadata|none"
    autoplay
    loop
    controls
  ></audio>
</body>
```

| 속성 이름 | 설명                                    |
| :-------: | :-------------------------------------- |
|    src    | 음악 파일의 경로 지정                   |
|  preload  | 음악을 재생하기 전에 모두 불러올지 지정 |
| autoplay  | 음악을 자동 재생할지 지정               |
|   loop    | 음악을 반복할지 지정                    |
| controls  | 음악 재생 도구를 출력할지 지정          |

### 7. 비디오 태그

```html
<body>
  <video
    src="Wildlife.mp4"
    poster="http://placehold.it/640x360"
    preload="auto|metadata|none"
    autoplay
    loop
    controls
  ></video>
</body>
```

| 속성 이름 | 설명                                      |
| :-------: | :---------------------------------------- |
|    src    | 비디오 파일의 경로 지정                   |
|  poster   | 비디오 준비중일때의 이미지 파일 경로 지정 |
|  preload  | 비디오를 재생하기 전에 모두 불러올지 지정 |
| autoplay  | 비디오를 자동 재생할지 지정               |
|   loop    | 비디오를 반복할지 지정                    |
| controls  | 비디오 재생 도구를 출력할지 지정          |
|   width   | 비디오의 너비 지정                        |
|  height   | 비디오의 높이 지정                        |

### 8. 입력 양식 태그

#### form 태그

```html
<body>
  <form action="/examples/media/action_target.php" method="get|post"></form>
</body>
```

| 속성 이름 | 설명                           |
| :-------: | :----------------------------- |
|  action   | 입력 데이터의 전달 위치를 지정 |
|  method   | 입력 데이터의 전달 방식을 선택 |

#### input 태그

```html
<body>
  <form>
    <input type="text" /><br />
    <input type="submit" /><br />
  </form>
</body>
```

|  type 속성값   | 설명                              |
| :------------: | :-------------------------------- |
|     button     | 버튼을 생성합니다.                |
|    checkbox    | 체크박스를 생성합니다.            |
|      file      | 파일 입력 양식을 생성합니다.      |
|     hidden     | 보이지 않습니다.                  |
|     image      | 이미지 형태를 생성합니다.         |
|    password    | 비밀번호 입력 양식을 생성합니다.  |
|     radio      | 라디어 버튼을 생성합니다.         |
|     reset      | 초기화 버튼을 생성합니다.         |
|     submit     | 제출 버튼을 생성합니다.           |
|      text      | 글자 입력 양식을 생성합니다.      |
|     color      | 색상 선택 양식을 생성합니다.      |
|      date      | 일 선택 양식을 생성합니다.        |
|    datetime    | 날짜 선택 양식을 생성합니다.      |
| datetime-local | 지역 날짜 선택 양식을 생성합니다. |
|     email      | 이메일 입력 양식을 생성합니다.    |
|     month      | 월 선택 양식을 생성합니다.        |
|     number     | 숫자 생성 양식을 생성합니다.      |
|     range      | 범위 선택 양식을 생성합니다.      |
|     search     | 검색어 입력 양식을 생성합니다.    |
|      tel       | 전화번호 입력 양식을 생성합니다.  |
|      time      | 시간 선택 양식을 생성합니다.      |
|      url       | URL 주소 입력 양식을 생성합니다.  |
|      week      | 주 선택 양식을 생성합니다.        |

#### textarea 태그

```html
<body>
  <form>
    <textarea cols="40" rows="5"></textarea>
  </form>
</body>
```

| 속성 이름 | 설명                      |
| :-------: | :------------------------ |
|   cols    | 태그의 너비를 지정합니다. |
|   rows    | 태그의 높이를 지정합니다. |

#### select 태그

```html
<body>
  <form>
    <select>
      <optgroup label="Coffee">
        <option value="espresso">에스프레소</option>
        <option value="americano">아메리카노</option>
      </optgroup>
      <optgroup label="Tea">
        <option value="earl grey">얼그레이티</option>
        <option value="jasmine">자스민티</option>
      </optgroup>
    </select>
  </form>
</body>
```

| 태그 이름 | 설명                    |
| :-------: | :---------------------- |
|  select   | 선택 양식을 생성합니다. |
| optgroup  | 옵션을 그룹화합니다.    |
|  option   | 옵션을 생성합니다.      |

### 9. 공간 분할 태그

```html
<body>
  <div>block</div>
  <div>block</div>
  <div>block</div>
  <hr />
  <span>inline</span>
  <span>inline</span>
  <span>inline</span>
</body>
```

```html
<body>
  <header>
    <h1>HTML5 Header</h1>
  </header>
  <nav>
    <ul>
      <li><a href="#">Menu1</a></li>
      <li><a href="#">Menu2</a></li>
      <li><a href="#">Menu3</a></li>
    </ul>
  </nav>
  <section>
    <article>
      <h2>1. Article</h2>
      <p>This is a article 1.</p>
    </article>
    <article>
      <h2>2. Article</h2>
      <p>This is a article 2.</p>
    </article>
  </section>
  <footer>
    <address>사랑시 고백구 행복동</address>
  </footer>
</body>
```

| 태그 이름 | 설명                                |
| :-------: | :---------------------------------- |
|    div    | block 형식으로 공간을 분할합니다.   |
|   span    | inline 형식으로 공간을 분할합니다.  |
|  header   | 헤더를 의미                         |
|    nav    | 내비게이션을 의미                   |
|  section  | 여러 중심 내용을 감싸는 공간을 의미 |
|  article  | 글자가 많이 들어가는 부분을 의미    |
|   aside   | 사이드에 위치하는 공간을 의미       |
|  footer   | 푸터를 의미                         |
