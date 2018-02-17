# github 사용하기
이 문서는 개발을 시작하는 주니어 개발자 및 프로그래머에게 요구되는 역량 중 하나인 버전관리와 버전관리시스템(VCS)의 대표적 예시인 깃(Git)을 쉽게 이해하고 실제로 적용할 수 있도록 돕기 위해 만들어진 문서입니다. 
일부 내용은 공식 Git Documentation을 참고하였습니다.

## 1. 시작하기
### 1.1 버전관리란 무엇인가
버전관리는 쉽게 말해 작성한 코드 또는 작업 결과물에 대한 변화 과정이나 변경 이력 또는 수정 내용을 기록해두는 것을 의미합니다. 
이러한 버전관리를 돕는 유용한 도구 중 하나가 Git이며 이것을 버전관리시스템, 줄여서 VCS라 부릅니다.

VCS를 사용하면 각 파일을 이전 상태로 되돌릴 수 있고, 프로젝트를 통째로 이전 상태로 되돌릴 수 있고, 시간에 따라 수정 내용을 비교해 볼 수 있고, 누가 문제를 일으켰는지도 추적할 수 있고, 누가 언제 만들어낸 이슈인지도 알 수 있죠. 
VCS를 사용하면 파일을 잃어버리거나 잘못 고쳤을 때도 쉽게 복구할 수 있습니다.

이러한 장점 때문에 VCS는 협업을 위한 최고의 툴이기도 합니다.

### 1.2 세가지 공간과 세가지 상태
Git을 사용하면서 머릿속에서 잊어서는 안되는 세가지 공간(Space)과 세가지 상태(State)가 있습니다. 

먼저, 공간은 Git 디렉토리(.git)와 스테이징 공간(Staging Area), 그리고 작업 디렉토리(Working Directory)가 있습니다. 

여러분의 작업 디렉토리에 깃을 설정(initialize .git)했다고 가정하죠.
로컬 컴퓨터에서 여러분이 코드를 작성하고 그것을 저장했다면 그 공간을 작업 디렉토리라고 할 수 있습니다. 이때 여러분의 파일은 Modified라는 상태와 함께 Unstaged의 상태를 가집니다.

Staging Area는 곧 커밋(Commit)하기 직전의 파일들의 정보를 저장하는 공간입니다. 이 Staging Area에 파일 Stage하여 커밋할 스냅샷을 만듭니다. 이때 파일은 Staged의 상태입니다.

이제 여러분의 작업 디렉토리 내에 위치한 .git 디렉토리로 커밋한다면 여러분의 새로운 버전이 생긴 것입니다.

## 2. 설치하기
### 2.1 Install
### Mac
```
$ brew install git
```
### Linux (Debian)
```
$ sudo apt-get install git-all
```
### Linux (Fedora)
```
$ sudo yum install git-all
```
### Windows
```
manual install
```

### 2.2 config
CLI에서 git 명령어를 입력하거나 git bash를 통해 실행합니다.
```
$ git config --global user.name "Juneyoung Kang"
$ git comfig --global user.email juneyoung_kang@outlook.com
```

## 3. Git 기초
### 3.1 깃 저장소 만들기
