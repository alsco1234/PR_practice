# PR_practice
## 2200080
- - -
### 1. git/github   
* **git** : 지역 저장소를 만들고 파일, 코드 등을 관리하는 작업(**편집기**)   
* **git hub** : 로컬에서 git으로 관리하는 자료를 다른 사람들과 공유하거나 백업해둘 수 있는 웹사이트(**공유 게시판**)   
* **git이 파일을 관리하는 상태**   
> * untracted : init   
> * modified   
> * staged : add   
> * commited : commmit   
- - -
### 2. Alias 설정 / Branch     
* **Alias** : 별명, 단축어   
> * vi 편집기 이용 (vi ~/.gitconfig)   
* **Branch** : 커밋들을 포인팅하는 포인터    
> * Branch 생성 : git branch "새브랜치이름"   
> * Branch 이주 : git checkout "이동할브랜치이름"   
> * Branch 확인 : git branch   
> * Branch 병합 : git merge "병합할브랜치이름" --> 브랜치를 현재의 브랜치로 병합   
> * Branch 기록확인 : git log   
> * 커밋 취소 : git reset   
> * **merge cinflict** :
<pre>
<code>
void message(){
  puts("branch is good");
 }
 void main(){
 <<<<<<<< HEAD
  puts("branch is good");
========
  message();
 >>>>>>>> testing
}
</code>
</pre>
HEAD에서 변경된 부분은 <<<HEAD에서 ===까지   
testing 브랜치에서 변경된 부분은 ====부터 >>>testing까지
