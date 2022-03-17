220317 Github 특강***

Mac은 Git 이 내장되어 있어 설치가 필요없다.

spotlight (**command + spacebar** : 검색) 을 열고 **terminal** 검색

terminal 창이 CLI(Command Line Interface)



## CLI 명령어

(데스크탑) 폴더 열기 : **open .**

항상 경로에 유의하기

- 새로운 폴더 생성 : **mkdir 폴더명**   (makingdirectory) 

ex.  mkdir test , mkdir 'hi hello'(띄어쓰기 있으면 따옴표)

- 경로를 바꿈. 디렉토리 변경 : **cd**  (change directory)

ex.  cd test

- 위치한 곳에 파일 만들기 : **touch** 

ex.  touch test.txt

- 위치한 곳 나가서 상위로 이동 : **cd ..**  (상대 경로의 일환)

- 가지고 있는 파일 전체 다 나옴. 파일이 있는지 확인하기 : **ls**  (list segments) 

**ls -a** 숨김파일까지 확인가능

- 폴더/파일 지우기 : **rm**  (remove)

ex. rm test.txt 

rm test 하면 directory 여서 삭제가 안된다고 뜸

그러면 폴더 지울때는 어떻게? **rm -r test** 

주의 rm을 사용해서 삭제하면 휴지통에 남지 않고 아예 삭제됨

강제삭제 : **-rf** 삭제를 하면 안되는 파일도 삭제하기 때문에 되도록 사용하지 않기

**command + l 한 줄 삭제**

- **mv** (move) 

ex. test directory 로 파일을 이동 : mv a.txt test

만약에 test2 directory가 없는데 test2로 이동해달라고 하면

( mv a.txt test2 ) 확장자 없이 이름을 바꿔버림

- 절대주소 : **pwd**

cd (절대주소)로 이동가능



## 마크다운

typora 이용해서 배움

**command + q**  typora 닫기

**command + ,**  typora 설정

**command + s**  저장

마크다운은 글에게 역할을 부여하는 것

**ctrl+/** 하면 원래 어떻게 썼는지 보임 (되돌리려면 다시)



- 제목

#제목1

##제목2

###제목3



- 목록

  - 순서가 없는 목록

    -목록

    ​	-서브목록 (**들여쓰기 tab**)

    ​		-서브 목록

    ​	-서브목록 (**내어쓰기 shift+tab**)

    -, *, + 표시

  - 순서가 있는 목록

    1.목록

    ​	1.서브목록

    ​	-서브목록

    2.목록
    
    

- 글꼴

굵게 : ** 글자**, __ 글자__ (typora 상에서만 command+b 가능)

**글자**

기울임 : * 글자* , _ 글자_ (typora 상에서만 command +i 가능)

*글자*

취소선 : ~~ 글자~~

~~글자~~ 

밑줄 : `<u> </u>` (typora 상에서만 command+u 가능) 

<u>글자</u>

- 코드

인라인코드 :  `inline code` (` 백틱에 감싸기)

블록코드 : ````python` 백틱 3번 입력하고 코드 종류 작성

```python
print('hello world')
      
```

 ````bash`

```bash
mkdir test
touch a.txt
```



- 링크

`[표시할 글자](주소)` 

[네이버](https://www.naver.com/)



- 이미지

`![표시할 글자](보여주고 싶은 사진 url)` 이미지 주소복사로 url 갖구오기

`![스크린샷 2022-03-18 오전 12.21.11](day01.assets/스크린샷 2022-03-18 오전 12.21.11.png)` 복사해서 command + v

![스크린샷 2022-03-18 오전 12.21.11](day01.assets/스크린샷 2022-03-18 오전 12.21.11-7530567.png)



`![농담곰 능이버섯](https://pbs.twimg.com/media/Eln4ROLVcAAplFi.jpg)`

![농담곰 능이버섯](https://pbs.twimg.com/media/Eln4ROLVcAAplFi.jpg)



- 인용

">" 사용

> 인용
>
> > 중첩된 사용
> >
> > > 가능



- 구분선 p`***``---``___` 3번 연속

---

***



- 표

타이포라에서 편하게 만들 수 있음

**option + command + t**

![스크린샷 2022-03-18 오전 12.27.42](day01.assets/스크린샷 2022-03-18 오전 12.27.42-7530892.png)

|      |      |      |
| ---- | ---- | ---- |
|      |      |      |
|      |      |      |
|      |      |      |



## GIT 기본 명령어

**VS 코드**

**cntl +` ** 터미널 열기

터미널에서 

X(닫기) 버튼은 터미널 내용은 유지하고 잠시 숨긴 것

휴지통 버튼은 터미널을 아예 삭제하는 것

경로조심 

![img](https://hphk.notion.site/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F572c62c6-15b4-4f94-bea1-ed308bcc9fdd%2FUntitled.png?table=block&id=8031afd1-69ff-4259-9b9a-e736278d888c&spaceId=daa2d103-3ecd-4519-8c30-4f55e74c7ef4&width=2000&userId=&cache=v2)

![img](https://hphk.notion.site/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Fc86c667a-616f-45b6-892e-15da6a3c494e%2FUntitled.png?table=block&id=9891aa63-a20f-43ea-949b-b41e4b62f1d0&spaceId=daa2d103-3ecd-4519-8c30-4f55e74c7ef4&width=2000&userId=&cache=v2)



**git init**  : git 으로 관리되게 하기, git repository(저장소)가 되었다

( **ls -a** 해서 **.  ..  .git** 나오면 잘된 것)

**git config --global user.name "kyee0423"** 

**git config --global user.email "kyee0423@naver.com"** 

**git config --global core.editor "code --wait"**

**git config --global --list**



**git add** : 무대에 올라갈 수 있게 추가해줘

touch README.md

ex. **git add** README.md

- 표시면 저장 안된거니까 command + s 로 중간 중간 저장해주기

**git status** 로 상태 확인해주기

**git commit -m "first commit"**  : " "로 변경사항 기록해줘

On branch master
nothing to commit, working tree clean

**git log --oneline** : 변경사항 한줄로 보여줘

**git add .**

**git commit -m "second commit"**




## GIT 연결하기

원격 저장소(repository) 만들고, 로컬과 연결하기

git init 통해서 TIL폴더를 로컬 저장소로 만듦

**git remote add origin** (깃 허브 원격 저장소 url) : 원격 저장소 등록

git remote add origin https://github.com/kyee0423/TIL.git

**git remote -v** : 원격 저장소 조회

git remote -v

origin https://github.com/kyee0423/TIL.git (fetch)

origin https://github.com/kyee0423/TIL.git (push)







push 통해서 기록(commits) 업로드
