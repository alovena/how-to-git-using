# how-to-git-using
 how to easy in a registered network
0. 참고 사이트

https://nolboo.github.io/blog/2013/10/06/github-for-beginner/

1. Git 설치하기

https://git-scm.com/downloads

사용 OS에 맞는 설치파일을 설치해 주세요~

설치 파일 실행하고 다 Next 눌러서 특별한 변경없이 설치했습니다

2. 로컬 저장소를 만들기 위한 준비!

깃에는 로컬 저장소와 원격 저장소가 있는데요

로컬 저장소는 개인적인 공간에 있는 저장소이기 때문에 다른 사람이 접근 할 수 없고

원격 저장소는 온라인으로 접근해야 하는 데스크탑 외부의 저장소로써 

다른 사람과 공유하며 사용할 수 있는 저장소입니다~


먼저 로컬 저장소를 만듭니다.

폴더를 새로 만들어서 업로드할 프로젝트를 복붙해서 넣거나

기존에 프로젝트가 있는 폴더를 그냥 사용해도 됩니다.


3. 그 상위폴더로 이동하여 로컬 저장소를 만듭니다.

상위 폴더에 오른쪽 마우스를 누르고 'Git Bash Here' 을 선택합니다.

커맨드 창이 뜨게 됩니다. 깃 명령어를 사용할 수 있는 상태로 만들어 줍니다

$ git init


4. 로컬 저장소에 파일 add하기

저장소는 생성되었지만 아직 어떤 파일을 올릴 지는 정해지지 않은 상태입니다.

status 명령어를 통해 현재 상태를 확인할 수 있습니다.

아직 모든 파일이 untracked 된 상태입니다.
$ git status


이제 add 명령어로 untracked 파일을 tracked 파일로 만들어줍니다!

저는 아까 세개의 폴더를 모두 add하도록 하겠습니다.

파일 하나만 할 수도 있어용

쭉쭉 작업이 실행됩니다.

$ git add 원하는파일/폴더이름

5. commit 하기 ( 현재 상태를 스냅샷처럼 저장하기! )

commit 명령어를 이용하여 원하는 메모와 함께 현재 상태를 저장합니다.

$ git commit -m "원하는 내용"

쭉쭉 작업이 시작됩니다.

작업이 끝나면 다시 status를 확인해 봅시당

Untracked files 목록에 좀전에 추가한 파일/폴더가 보이지 않습니당!!

6. 원격 저장소로 연결하기

이제 로컬 저장소의 변경사항을 원격 저장소로 연동합니다! 드디어 GitHub에 올라갈 차례입니당

깃허브에서 저장소를 하나 만들고 저장소 연결 주소를 하나 얻어옵니다.

저는 https://github.com/imdasom/moonzigi.git 이거에용


$ git remote add origin https://github.com/imdasom/moonzigi.git

$ git remote -v


7. push하여 원격 저장소로 commit 내용 올리기!

이제 push 명령어를 사용하여 원격 저장소 origin으로 commit했던 내용을 갱신합니다.

$ git push origin master

8. 깃허브에서 확인하기

제대로 올라간 것을 확인해보세용!!

아까 add하고 commit한 내용들이 올라가 있습니당

다만 함정이라면 모든 commit 내용이 똑같다는거..ㅋㅋ

add하고 원하는 내용으로 commit하고 반복해서 그런식으로 했어야 되는데

첨이라 잘 못햇네영ㅋㅋㅋㅋ 아무튼 끝!!! 담엔 안드로이드 스튜디오와 연동해서

더욱 편리하게 관리해보도록 하겠습니당

