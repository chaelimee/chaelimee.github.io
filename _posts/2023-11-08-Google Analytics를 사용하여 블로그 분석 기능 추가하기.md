---
layout: post
title:  "Google Analytics를 사용하여 블로그 분석 기능 추가하기"
date:   2023-11-08 17:26:29 +0900
categories: Blog_Making
published: true
---
블로그라는 것은 누구나 접할 수 있는 사이트입니다. 지금 저의 블로그는 모두 한국어로 되어있어 저의 블로그를 접속하는 사용자가 대부분 한국인일테지만, 만약 영어로 작성한 글이 있다면 외국인이 유입되는 상황이 생기게 될 것입니다. 그래서 이번에 추가해볼 기능은 바로 내 블로그에 어느 나라 사람이!! 우리나라의 어느 지역 사용자가!! 다녀갔는지 조회를 해 볼 수 있는 분석 기능입니다. 자 이제 시작해보겠습니다.

___
<br>


# 첫번째, Google Analytics 계정 설정하기 <br/>

<img src="/images/ga1.png"><br/>

### 1️⃣ 일단 [Google Analytics](https://analytics.google.com)에 접속을 하여 google 계정 로그인을 해줍니다. 그리고 측정 시작 버튼을 눌러줍니다.
<br/><br/><br/><br/>

<img src="/images/ga2.png"><br/>

### 2️⃣ 계정을 생성하는 단계에서 계정 이름을 적어줍니다.

사용자명으로 적어주시면 됩니다.
<br><br><br><br>

<img src="/images/ga3.png"><br/>

### 3️⃣ 다음 속성 만들기 단계에서는 속성 이름을 사용자명.github.io로 설정합니다. 그리고 보고 시간대와 통화는 '대한민국/대한민국 원(₩)'으로 설정합니다.
<br/><br/><br/><br/>

<img src="/images/ga4.png"><br/>

### 4️⃣ 자신의 옵션대로 업종 카테고리를 선택하고 비즈니스 규모를 선택합니다.
<br/><br/><br/><br/>

<img src="/images/ga5.png"><br/>

### 5️⃣ 여러 항목 중 자신의 비즈니스 목표를 선택합니다.
<br/><br/><br/><br/>

<img src="/images/ga6.png"><br/>

### 6️⃣ 이제 데이터를 수집할 준비가 되었습니다. 플랫폼을 선택하는데, 저는 웹에서 사용할 것이기 때문에 웹을 선택했습니다.
<br/><br/><br/><br/>

<img src="/images/new.png"><br/>

### 7️⃣ 다음은 데이터 스트림을 설정할 차례입니다. 웹사이트 URL 항목에 자신의 깃허브 링크를 작성한 후 스트림이름을 적어줍니다. 
<br/><br/><br/><br/>

# 두번째, Jekyll 블로그에 추적 코드 추가하기 

<br/>

### 1️⃣ VSCode를 열어 _config.yml 파일을 열어 analytics 관련 설정이 있는지 찾아봅니다. 만약 관련 설정이 있다면 적절하게 수정해줍니다.
<br/><br/>

### 2️⃣ _config.yml 파일에 Google Analytics 추적 코드를 포함하는 설정이 없다면 직접 HTML 파일을 설정해야하는데요, 보통 _includes 폴더 내에있는 head.html 파일을 사용합니다.
<br/><br/>

<img src="/images/codee.png"><br/>

### 3️⃣ head.html 파일을 열고 아까 생성한 코드를 복사하여 </head> 태그 앞에 붙여넣어줍니다.
<br/><br/><br/><br/>

<img src="/images/head.png"><br/>

#### 저같은 경우에는 _config.yml 파일에 analytics 관련 설정이 없어서 직접 HTML 파일을 설정했습니다.
<br><br>

### 4️⃣ 수정한 내용을 저장한 후 Github에 커밋과 푸시를 해줍니다.

```
git add .
git commit -m "커밋 메세지"
git push
```
<br><br>

## 세번째, 이 모든 설정을 마쳤다면 Google Analytics 사용하기 

<br>

### 추적 코드 스트립트가 head.html 파일에 정상적으로 추가 되었다면 Google analytics 대시보드-보고서 개요-실시간 탭에서 실시간 사용자를 확인할 수 있습니다.

<br><br><br>

___
<br>

아직은 한국어로만 글을 작성하고 있지만, 나중에 개발 중 오류가 발생했을때 그 오류를 해결하는 과정을 블로그에 작성한다면, 같은 오류를 해결하려는 사람이 구글링해서 우연히 제 블로그를 볼지도 모릅니다. 그때 이 기능을 사용할 수 있겠죠? 우리나라가 아닌 외국에서 제 블로그를 보는 사람이 있다면, 정말 신기하면서도 동시에 뿌듯할 것 같네요. 그 날이 올때까지 저도 열심히 개발해보겠습니다!! 
