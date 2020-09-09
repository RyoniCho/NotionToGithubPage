# NotionToGithubPage

## 1. Notion To Github page?

Notion에서 작성한 페이지를 GitHub Pages 기반(jekyll) 블로그의 형식에 맞게 변환해주는 파이썬 스크립트입니다. 
[uoneway님의 프로젝트](https://github.com/uoneway/Notion-to-GitHub-Pages)를 참고하여 만들어졌습니다.(감사합니다)

## 2. 기능

- Notion에서 export한 markup 파일 및 이미지 폴더를 GitHub Pages의 Jekyll서비스의 post 형식에 맞게 이름 및 경로를 변환해줍니다.
    - image폴더내의 이미지파일은 *assets/images/posts/{입력받은타이틀}* 폴더로 이동됩니다.
    - md파일 내 image 경로또한 이에 맞게 수정됩니다.
    - md파일은 파일명을 *날짜-{입력받은 타이틀}.md*로 변환합니다.
    - front matter는 커스텀txt파일에 적은내용으로 md파일에 반영합니다. 

    

## 3. 사용방법

1. python 3.x버전 설치가 필요합니다. 

2. ***notionToGithubPage.py*** 파일과 ***customFrontMatter.txt*** 을 다운로드하여, 로컬PC의  GitHub Pages root 폴더(이하 *GitHub Pages root*)로 옮깁니다.

3. Notion app에서 GitHub Pages에 업로드하고자 하는 Notion 노트를 *Markdown & CSV* 형식으로 export합니다.

4. Notion에서 export한 zip 파일을 본인 local PC의 *GitHub Pages root* 경로로 옮깁니다.

5. ***customFrontMatter.txt*** 파일을 열어 해당 포스트의 Front Matter 정보를 수정합니다(타이틀과 날짜는 포함안됨)

6. Local 컴퓨터의 Shell에서 *GitHub Pages root* 경로로 이동 후, 다음을 입력합니다.

        python notionToGithubPage.py

7. 타이틀과 날짜정보를 입력합니다.

8. 이 과정이 끝나면  *날짜-{입력받은 타이틀}.md* 이 생성되며 관련 이미지파일은 *assets/images/posts/{입력받은타이틀}* 폴더로 이동됩니다. md파일만 _post폴더내 원하는곳으로 옮겨주시면됩니다.



피드백 및 문의, fork 언제나 환영합니다 :)