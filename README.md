# 0709 강의 회고

## 1. 파이썬 설치

3.12.7 버전을 설치함.

Add python.exe to PATH를 해줘야함

버전확인은 맥은 
python3 --version
pip --version

처음에 깐 파이썬은 대가리 같은것. 이걸 프로젝트에 갖다 쓰지않음.

프로젝트별로 .venv를 만들어서 거기서 돌린다.


## 2. vscode, github

vscode는 깔고, github 계정으로 로그인해둔다.
확장프로그램들을 깔아준다.

p.s 맥은 zsh를 사용중이라 powershell과 다른점이 있음.

Git 최초 1회 설정
git config --global user.name "이름"
git config --global user.email "이메일"

처음에 이걸 해줘야, 누가 커밋푸시하는지 저장됨.
여기서 깃허브를 커밋하고 푸시하는 과정이 있다.

git 과 github는 다름. 
git은 로컬에 커밋하면 저장되는 파일
github에는 푸시가 돼야 올라감.

pull은 다른 사람이 뭔가 추가했을 때, 그 추가된 파일만 내가 끌어온다.

(이 기능들로 기록, 버전 관리, 협업이 가능)

.gitignore 로 깃허브에 푸시되지 않도록 하는 리스트를 만들어둔다. .venv 같은건 넣을 필요가 절대 없음
깃허브에는 명세서와 같은 코드만 들어가면됨.

레포지터리는 settings 에서 함.

## 3. venv

설치하려는 폴더에 가서 통합터미널 open
python -m venv .venv
로 설치

-m은 권한 문제 있으면 해야됨. .venv는 그냥 아무이름으로 만든다는 뜻.

가상환경 활성화를 해줘야된다.

source .venv/bin/activate
를 하면 앞에 .venv가 보인다. zsh 일 경우 오른쪽에 초록글씨로 표시되기도함.

여기에도 pip 업글을 돌려줘야함.
pip -m pip install --upgrade pip

pip install -r requirements.txt
요건 venv 안에 약간 파이썬 설치한 것에 없는 것들을
넣는 과정이다. 각 프로젝트마다 다를것. txt 파일 안에
넣는다.