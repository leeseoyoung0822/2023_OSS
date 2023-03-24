# 2023_OSS
## 2023 OSS 수업 

-----
### 3주차 git

### 이미지
![kau](https://user-images.githubusercontent.com/105160895/227480566-5c4706f9-4008-4ed0-a5be-383bce896b1f.png)



### 링크   
[LMS](https://lms.kau.ac.kr "항공대학교 강의관리시스템")

#### ProGit 링크
[ProGit](https://git-scm.com/book/ko/v2 "git 문서, 한국어")


##### 주요 git 명령어
* add : 파일을 추적 대상으로 포함시킬 때, 또는 커밋 대상으로 포함시킬 때 사용
    * 예) git add <file name>
* commit
* git reset HEAD <file> : stage된 파일을 unstaged로 변경
* git checkout -- <file> : stage되어 있는 파일을 수정한 후 수정 전으로 되돌림 
* branch
* merge
* status
* log
    * 예) git log --oneline --decorate --graph --all

------
### 2주차 숙제

```bash
#!/bin/sh

a=이서영
b=2020125046

echo "____________________"
echo "name :"
echo "$a"

echo "____________________"
echo "student id :"
echo "$b"

echo "____________________"
echo "file path : "
find /home/kau2 -name  "w2_homework.txt" 2>/dev/null

echo "____________________"
echo "line number : "
realpath=$(find /home/kau2 -name "w2_homework.txt" 2>/dev/null)
row=$(wc -l < "$realpath")
echo "$row"

echo "____________________"
echo "lask line : "
last=$(tail -n 1 "$realpath")
echo "$last" 

```

## 마크다운
### 목록
#### 번호 있는 목록 : 내림차순 정렬
1. 첫번째
3. 세번째
2. 두번째

#### 번호 없는 목록 : *, -, +
* 첫번째
- 세번째
+ 두번째
-----
* 빨강
  * 녹색
    * 파랑

### 강조
*single asterisks*    
_single underscores_    
**double asterisks**    
__double underscores__    
~~cancelline~~    
