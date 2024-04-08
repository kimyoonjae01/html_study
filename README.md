# Visual stydiocode (VScord)
* vss code 실행 시 가장 먼저 확인해야할 것!
* 왼쪽 탐색기가 당일 작업폴더로 연결되어 있는지 확인!
* (위) 안되어있다면 -> 파일 -> 작업폴더닫기 후 - 폴더열기 다시진행
# html 시작
* git, gitHub 개념공부
* `<태그>` 웹페이지에서 의미적인 정보를 대상
## HTML5 버전선언
* `<!doctype html>`
## html 구조태그
* html : 웹의 시작과 끝. 문서 자체 의미
* head : 웹 문서의 정보 , 제목포함
* meta : 웹 문서의 정보 기록
* title : 웹 문서의 제목(브라우저 상단표시)
* body : 웹 문서 내용(실제 대부분의 서비스가 들어가는 본문)
## 구조 태그 속성
* `iang='ko'` htmi문서 언어설정
* `charset='utf-8'` 다국어 문자열 설정
* `description` 사이트 요약 설명
* `ketwords` 사이트 검색 키워드 설정
## 속성 문법
* `<태그 속성='값' 속성='값'></태그>`
* 태그와 속성 사이 공백
* 속성과 속성 사이 공백(속성개수 제한없음)
* 속성은 시작태그에만 작성하기!
## 구조태그의  'tltle' 작성방법
* 메인페이지 -> 사이트명 
* 메인페이지 -> 사이트명 | 광고문구 추가 
* 서브페이지 -> 페이지명 | 사이트명
* ex) 책이름-저자명| 서점명 
* ex) 판매아이템명 | 사이트명
## h1~h6 제목 태그 (block tag)
* h1~h3 태그는 mata ketwords와 동일한 검색키워드로 활용된다. (대제목일수록 높음)
* h4~h6 태그는 거의 사용하지 않는다.
* h1은 대제목 사이트의 로고 및, 서브 페이지 제목에서 주로 사용한다
* h 제목의 1~6레벨은 순서대로 작성해야한다.
## 단락p(block tag) 글내용
* 한 줄 또는 여러 줄 단락 묶을 때 사용하는 태그
* 제목 (h) 태그 종류와는 형제 태그 관게로 사용해야한다. 부모-자식(x)
## inline 태그 br.eb.storng,del,s,sup,sub
* `br`: 블록 내 줄 바꿈
* `em`: 블록 내 강조 태그, 주로 내용 태그(p) 등에서 자식으로 사용
* `strong`: 블록 내 경고용 강조 태그(위와 특징통일)
* `del`: 삭제 텍스트, 쇼핑몰의 할인 전 가격 등에 사용
* `s`: 교체 텍스트, 쇼핑몰의 할인 전 가격 등에 사용(del) 자주사용
* `sup,sub`: 윗첨자(sup) 아래점차(sub) 수학, 과학 등의 기호에 사용
## 인용문 처리 blockquote , q
* `blockquote(block)` 단락 자체가 인용문에 해당할 때 사용 q태그와 부모-자식 관계로 사용해선 안된다
* `q(inline)` 단락(P)내에서 일부가 인용문에 해당할 때 사용
* 공통속성 `"cite='url"` : `blockquote`, `q`로 인용문 처리할 경우 출처 표시용도로 주소 (url)을 담아주는 속성 
## 특수문자 태그
* `&lt` 열기 `&gt;` <> 이게 됌
* `&copy;` C모양 아이콘
* `&reg` R모양 아이콘
* `&` 시작 `;` 종료
* `&copy` &시작과 copyright의 copy; 종료
## 주소 태그
* `address` 웹사이트의 연락처, 소개, 고객센터 정보 등을 담을 때 사용합니다
*  footer 영역의 주로 사용합니다.
* `p` 안에 넣을 수 없음
## 수평선 태그 `hr` 수평선
* 사이드 각 영역을 구분할 때 사용
* css 에서는 표현하지 않고 숨기는 경우가 대부분
* 주석과 같이 태그 구조 이해에 주 용도로 사용합니다
## 컴퓨터 명령어 태그
* `code` inline 웹 강의 사이트에서 주로 사용하는 태그
## 링크태그 a
* block, inline 특징을 모두 가진다.
* 절대경로와 상대경로를 href 속성에 작성한다
* 상대경로는 a태그 작성중인 파일 위치 기준 연결하고자 하는 목적지파일이 같은 위치에 있는지, 하위 위치에 있는지, 상위 위치에 있는지에 따라 다르게 작성한다.
* ./ 현재 위치에서 시작
* ../ 상위 폴더로 나가기
* `./doll.jpg` : 현재 위치에서 dell.jpg 파일 찾기
* `../dell.jpg` : 상위 폴더로 한단게 나가서 doll.jpg파일 찾기
* `../a/doll.jpg` : 상위폴더로 한단계 나가고 a 폴더로 들어가서 dell.jpg 파일 찾기
* `./b/doll.jpg` : 현재 위치에서 b폴더로 들어가서 dell.jpg 파일 찾기
* 나가야함 ../ , 두번 나가야함 ../../ 
* 이 위치에 있음 ./파일명 
* 이 위치에 있는 폴더 안에 있음 ./폴더/파일명
* 이 위치에 폴더 안에 안에 있음 ./폴더./폴더./파일명
## 바로가기 링크란?
* 단순 페이지 이동이 아닌 특정 위치로 스크롤 이동하는 바로가기 기능
* ex- `<a href='#1'>` 1번링크로 가기   / 클릭시 1번링크로 바로 스크롤 내려감
* ex- `<h1 id='1'>`1번링크</h1>
## 바로가기 링크 제작 순서 및 주의사항
*  #태그 위치 순서 잘보기
1. 이동목적지에 가장 가까운 태그에`id`를 적용한다.
2. 링크 대상에 `#id` href 속성값에 담기
* 주의사항 : `#`은 아이디 링크에만 사용할 것
## 파비콘 적용 순서
1. 파비콘 크기로 이미지 다운받거나 편집하기
2. html에서 `head`안에 link태그로 파비콘 주소 연결하기
* <link rel="shortcut icon" href="파비콘.ico 경로" type="image/x-icon">
<link rel="icon" href="파비콘.ico 경로" type="image/x-icon">
* 파비콘.ico 경로에 <./> 으로 넣는다
## 이미지태그 `img`
* <img src="url" alt=""> 기본태그
* 이미지 사용 시 의미전달이 필요한 이미지인지 필요하지 않은 이미지인지 구분해야한다.
* ex <p><a href="#"><img src="./image_video/images/aoa_banner.jpg" alt="접근성 오픈 아카데미 유투브 채널 . 매주 월요일 컨텐츠 업데이트"></a></p>
## 비디오태그
* 작성방법 1 
<video src=”동영상경로”></video> autoplay,loop,muted 속성 잊지말기
작성방법2
* <video>
* <source src=’동영상경로’ type=’동영상타입1’> 속성 잊지 말기 
## fighure, figcaotion / 이미지 누르든 글 누르든 똑같은 곳으로 가기
* 문서 안 사진을 감싸는 틀로서 활용하고 사진의 캡션을 정의할 수 있음
* <figure>
<img src=”URL” alt””>
<figcaption>신혼일기</figcaption>
<figcaption>자까</fogcaption>
## 이미지 태그'img' inline
* <img src='' alt=''>
* alt 는 시각장애인이 편견없이 정보확일할 수 있도록 한다.
* src 부분에 './' 이렇게 시작하면 현재폴더에서 상위로만 가능
* '../' 이렇게 시작하면 하위폴더로 나갈 수 있음