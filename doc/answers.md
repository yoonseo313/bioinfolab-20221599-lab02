# Codespace 사용 확인 답안
 
학번 : 20221599
이름 : 장윤서
 
## 2-1. 아이콘 정리
 
| 순서 | 아이콘 이름 | 모양 | 하는 일 |
|------|-------------|------|---------|
| 1 |  탐색기  | 종이 모양 |폴더와 파일 목록을 보여주고, 생성, 삭제 및 이름 변경 |
| 2 |  검색  | 돋보기 모양 |프로젝트 전체 파일 내에서 특정 단어나 문장을 한 번에 찾아줌 |
| 3 |  소스 제어  | 동그라미로부터 가지가 뻗는 모양 |Git을 이용해 코드의 변경 이력을 관리, Commit이나 Github push,pull기능 |
| 4 |  실행 및 디버그  | 세모 위에 벌레가 있는 모양 |작성한 코드를 실행 및 오류를 찾아냄 |
| 5 |  확장  | 블록 네개가 모인 모양 |파이썬, 주피터 등 프로그래밍에 필요한 추가도구를 설치 및 사용가능하도록 함 |

 
## 2-2. 가. 파일 탐색기
터미널에서 ls 실행 시 폴더가 보임
@yoonseo313 ➜ /workspaces/bioinfolab-20221599-lab02 (main) $ ls lab02
ls: cannot access 'lab02': No such file or directory
@yoonseo313 ➜ /workspaces/bioinfolab-20221599-lab02 (main) $ ls
data  doc  LICENSE  README.md  src  test 

## 2-2. 나. 검색
**검색어 Alice**
Aa 옵션 켰을 때 : 399 results in 1 file
Aa 옵션 껐을 때 : 399 results in 1 file
**완전한 검색어 alice**
ab 밑줄 켰을 때 : 385 results in 1 file
**완전하지 않은 단어 ali 로 검색 시**
ab 밑줄 켰을 때 : 406 results in 2 files
- 다른 이유 :  

**lab02 포함 시 명령어 아래에서 결과값을 찾지못함, data파일내에서 셀수있음**
@yoonseo313 ➜ /workspaces/bioinfolab-20221599-lab02 (main) $ grep -o -i "Alice" lab02/data/alice.txt | wc -l
grep: lab02/data/alice.txt: No such file or directory
0
@yoonseo313 ➜ /workspaces/bioinfolab-20221599-lab02 (main) $ grep -o -i "Alice" data/a
lice.txt | wc -l
399

## 2-2. 다. 소스 제어
@yoonseo313 ➜ /workspaces/bioinfolab-20221599-lab02 (main) $ git log -1
commit 08f5aca191e897483ce75614be9f4caed560f77c (HEAD -> main, origin/main, origin/HEAD)
Author: CHANG Yoon Seo <20221599@sungshin.ac.kr>
Date:   Tue Sep 8 05:14:07 2026 +0000

    update
    
## 2-2. 라. 확장
**Python**
- 버전 : 2026.4.0
**Jupyter**
- 버전 : 2025.9.1
