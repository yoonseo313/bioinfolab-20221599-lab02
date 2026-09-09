# Codespace 사용 확인 답안
 
학번 : 20221599
이름 : 장윤서
 
## 2-1. 아이콘 정리
 
| 순서 | 아이콘 이름 | 모양 | 하는 일 |
|------|-------------|------|---------|
| 1    | 탐색기 | 종이 모양 | 폴더와 파일 목록을 보여줌, 파일을 생성 및 삭제, 이름변경이 가능한 곳 |
| 2    | 검색 | 돋보기 모양 | 프로젝트 파일 내에서 특정 텍스트를 찾을 수 있음 |
| 3    | 소스 제어 | 동그라미로부터 가지들이 뻗어가는 모양 | Git으로 변경된 파일을 확인하고, 스테이징, commit, push 등을 할수있음 |
| 4    | 실행 및 디버그 | 세모 위에 벌레가 있는 모양 | 코드를 실행하거나, 중단점을 걸어 한줄씩 실행하며 오류를 찾는 디버깅 기능 |
| 5    | 확장 | 블록 네개가 모인 모양 | python, jupyter 같은 확장 프로그램을 설치, 관리하는 곳 |
 
## 2-2. 가. 파일 탐색기
 data  doc  src  test

## 2-2. 나. 검색
 - Aa off : 400 results in 2 files
 - Aa on : 399 results in 1 file
 - ab 밑줄 on : 399 results in 2 files
 - 완전하지 않은 단어 : no results
 $ grep -o -i "Alice" lab02/data/alice.txt | wc -l
399
같은 결과가 나왔다. Aa 설정을 켰을때 대소문자를 구분해 Alice 를 검색하는데, alice.txt 에서는 대소문자 차이로 추가 검색되는 항목이 없어 결과가 399개로 동일하다. Aa 설정을 껐을때는 대소문자를 구분하지 않고 검색하면서, alice.txt 외에 다른 파일에서도 1개가 추가로 검색됐기 때문이다. 
## 2-2. 다. 소스 제어
 commit c4ea0cb7ef7a61cef3e1b8e604e1c1f1c6cac91d (HEAD -> main)
Author: CHANG Yoon Seo <20221599@sungshin.ac.kr>
Date:   Wed Sep 9 01:11:20 2026 +0000

    update
화면이 더 편했다. 변경된 파일 목록이 한눈에 보이고, 더하기 버튼 클릭만으로 스테이징이 되며, 커밋 메세지도 별도의 문법에 신경 쓸 필요없이 입력창에 바로 쓸 수 있어 실수하거나 에러가 발생하지 않고 커밋할 수 있어서 더 편하다고 느꼈다. 
## 2-2. 라. 확장
**Python** 버전 : 2026.4.0
**Jupyter** 버전 : 2025.9.1
미리 강의자가 설치해둔 확장인 것이라고 생각한다. .devcontainer 폴더 내에 devcontainer.json 파일 속 코드를 보면 "customizations": {
    "vscode": {
      "extensions": ["ms-python.python", "ms-toolsai.jupyter"],
 이라는 코드가 있는데 이 항목이 해당 확장들을 커스텀해서 vscode에 설치하는 코드라고 판단했다. 