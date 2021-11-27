## Git

[Git에서 커밋 메시지를 작성하는 명령어는 무엇인가요?](#Git에서-커밋-메시지를-작성하는-명령어는-무엇인가요)

[Git과 SVN의 차이점은 무엇입니까?](#Git과-SVN의-차이점은-무엇입니까)

[Git이란?](#Git이란)

[Git에서 가장 최근 커밋을 취소하는 방법은 무엇입니까?](#Git에서-가장-최근-커밋을-취소하는-방법은-무엇입니까)

[Git 포크란 무엇입니까? 포크, 분기 및 복제의 차이점은 무엇입니까?](#Git-포크란-무엇입니까-포크-분기-및-복제의-차이점은-무엇입니까)

["git pull"과 "git fetch"의 차이점은 무엇입니까?](#git-pull과-git-fetch의-차이점은-무엇입니까)

["풀 리퀘스트"와 "브랜치"의 차이점은 무엇입니까?](#풀-리퀘스트와-브랜치의-차이점은-무엇입니까)

[중앙 집중식 워크플로는 어떻게 작동합니까?](#중앙-집중식-워크플로는-어떻게-작동합니까)

[로컬 저장소를 업데이트해야 합니다. 어떤 git 명령을 사용할 것인가?](#로컬-저장소를-업데이트해야-합니다-어떤-git-명령을-사용할-것인가)

[이전 커밋으로 롤백해야 하며 최근 변경 사항은 신경 쓰지 않습니다. 어떤 명령어를 사용해야 할까요?](#이전-커밋으로-롤백해야-하며-최근-변경-사항은-신경-쓰지-않습니다-어떤-명령어를-사용해야-할까요)

["git cherry-pick"이란 무엇입니까?](#git-cherry-pick이란-무엇입니까)

[Git에서 작업 트리와 인덱스인 HEAD의 차이점을 알려주세요.](#Git에서-작업-트리와-인덱스인-HEAD의-차이점을-알려주세요)

["git stash"는 언제 사용해야 하나요?](#git-stash는-언제-사용해야-하나요)

[git에서 이전 커밋을 되돌리는 방법은 무엇입니까?](#git에서-이전-커밋을-되돌리는-방법은-무엇입니까)

[Forking Workflow의 장점 설명](#Forking-Workflow의-장점-설명)

[Gitflow 워크플로를 설명해 주시겠습니까?](#Gitflow-워크플로를-설명해-주시겠습니까)

["Rebase Workflow"에 대한 일련의 git 명령을 작성하십시오.](#Rebase-Workflow에-대한-일련의-git-명령을-작성하십시오)

[Git에서 "HEAD"는 무엇입니까?](#Git에서-HEAD는-무엇입니까)

[파일 시스템에서 파일을 제거하지 않고 git에서 파일을 제거하는 방법은 무엇입니까?](#파일-시스템에서-파일을-제거하지-않고-git에서-파일을-제거하는-방법은-무엇입니까)

["gitstash pop"과 "git stash apply"는 "gitstash 팝"의 git 은 영구적인가요?](#gitstash-pop과-git-stash-apply는-gitstash-팝의-git-은-영구적인가요)

["git reset"이 일반 영어로 무엇을 하는지 설명할 수 있습니까?](#git-reset이-일반-영어로-무엇을-하는지-설명할-수-있습니까)

[두 커밋의 차이점을 확인하기 위해 git 명령을 작성하십시오.](#두-커밋의-차이점을-확인하기-위해-git-명령을-작성하십시오)

[이전 Git 커밋을 수정하는 방법은 무엇입니까?](#이전-Git-커밋을-수정하는-방법은-무엇입니까)

[특정 파일의 특정 줄을 누가 변경했는지 알기 위해 어떤 git 명령을 사용해야 합니까?](#특정-파일의-특정-줄을-누가-변경했는지-알기-위해-어떤-git-명령을-사용해야-합니까)

["git merge" 대신 "git rebase"를 언제 사용합니까?](#git-merge-대신-git-rebase를-언제-사용합니까)

[git rebase를 쉽게 취소하는 방법을 알고 있습니까? ](#git-rebase를-쉽게-취소하는-방법을-알고-있습니까-)



### Git에서 커밋 메시지를 작성하는 명령어는 무엇인가요?

Use:
```sh
git commit -a
```

 -a on the command line instructs git to commit the new content of all tracked files that have been modified. You can use 
```sh
git add <file>
```
or 
```sh
git add -A
```

git commit -a 전에 새 파일을 처음으로 커밋해야 하는 경우.


###### Source

* https://www.edureka.co/blog/interview-questions/git-interview-questions/

[[↑] 맨 위로](#Git)
### Git과 SVN의 차이점은 무엇입니까?

Git 대 SVN 논쟁의 요점은 다음과 같습니다. Git은 DVCS(분산 버전 제어 시스템)인 반면 SVN은 중앙 집중식 버전 제어 시스템입니다.

###### Source

* https://medium.com/@gauravtaywade/15-interview-questions-about-git-that-every-developer-should-know-bcaf30409647

[[↑] 맨 위로](#Git)
### Git이란?

Git은 DVCS(Distributed Version Control System)입니다. 파일에 대한 변경 사항을 추적할 수 있으며 특정 변경 사항으로 되돌릴 수 있습니다.

분산 아키텍처는 SVN과 같은 다른 VCS(버전 제어 시스템)에 비해 많은 이점을 제공합니다. 한 가지 주요 이점은 프로젝트 파일의 모든 버전을 저장하기 위해 중앙 서버에 의존하지 않는다는 것입니다.

###### Source

* https://www.edureka.co/blog/interview-questions/git-interview-questions/

[[↑] 맨 위로](#Git)
### Git에서 가장 최근 커밋을 취소하는 방법은 무엇입니까?

```sh
$ git commit -m "Something terribly misguided"      
$ git reset HEAD~                                   # copied the old head to .git/ORIG_HEAD
<< edit files as necessary >>                       
$ git add ...                                       
$ git commit -c ORIG_HEAD                           # will open an editor, which initially contains the log message from the old commit and allows you to edit it
```

###### Source

* https://stackoverflow.com/questions/927358/how-to-undo-the-most-recent-commits-in-git

[[↑] 맨 위로](#Git)
### Git 포크란 무엇입니까? 포크, 분기 및 복제의 차이점은 무엇입니까?

* **fork**는 원본과 다른 저장소의 원격 서버측 복사본입니다. 포크는 실제로 Git 개념이 아니라 정치적/사회적 아이디어에 가깝습니다. 
* **clone**은 포크가 아닙니다. 클론은 일부 원격 저장소의 로컬 복사본입니다. 복제할 때 실제로 모든 기록 및 분기를 포함하여 전체 소스 저장소를 복사하는 것입니다.
* **branch**는 단일 저장소 내에서 변경 사항을 처리하여 최종적으로 나머지 코드와 병합하는 메커니즘입니다. 분기는 저장소 내에 있는 것입니다. 개념적으로는 개발 스레드를 나타냅니다.

###### Source

* https://stackoverflow.com/questions/3329943/git-branch-fork-fetch-merge-rebase-and-clone-what-are-the-differences/

[[↑] 맨 위로](#Git)
### "git pull"과 "git fetch"의 차이점은 무엇입니까?

가장 간단한 용어로 `git pull`은 `git fetch` 다음에 `git merge`를 수행합니다.

* `pull`을 사용하면 Git이 자동으로 작업을 수행하려고 합니다. **상황에 민감합니다**, 그래서 Git은 현재 작업 중인 브랜치에 가져온 커밋을 병합합니다. `pull` **먼저 검토하지 않고 커밋을 자동으로 병합합니다**. 지점을 잘 관리하지 않으면 자주 충돌할 수 있습니다.

* 'fetch'하면 Git은 현재 브랜치에 없는 대상 브랜치에서 커밋을 수집하여 **로컬 저장소에 저장합니다**. 그러나 **현재 브랜치와 병합하지 않습니다**. 이것은 리포지토리를 최신 상태로 유지해야 하지만 파일을 업데이트하면 손상될 수 있는 작업을 하는 경우에 특히 유용합니다. 커밋을 마스터 브랜치에 통합하려면 `merge`를 사용합니다.

###### Source

* https://stackoverflow.com/questions/292357/what-is-the-difference-between-git-pull-and-git-fetch

[[↑] 맨 위로](#Git)
### "풀 리퀘스트"와 "브랜치"의 차이점은 무엇입니까?

* **branch**는 코드의 별도 버전입니다.

* **pull request**은 누군가가 저장소를 가져오고 자신의 분기를 만들고 일부 변경을 수행한 다음 해당 분기를 병합하려고 시도하는 경우입니다(변경 사항을 다른 사람의 코드 저장소에 넣음).

###### Source

* https://stackoverflow.com/questions/19059838/whats-the-difference-between-a-pull-request-and-a-branch

[[↑] 맨 위로](#Git)
### 중앙 집중식 워크플로는 어떻게 작동합니까?

**Centralized Workflow**는 중앙 저장소를 사용하여 프로젝트의 모든 변경 사항에 대한 단일 지점 역할을 합니다. 기본 개발 분기를 마스터라고 하며 모든 변경 사항이 이 분기에 커밋됩니다.

개발자는 중앙 저장소를 복제하여 시작합니다. 프로젝트의 자체 로컬 복사본에서 파일을 편집하고 변경 사항을 커밋합니다. 이러한 새 커밋은 로컬에 저장됩니다.

공식 프로젝트에 변경 사항을 게시하기 위해 개발자는 로컬 마스터 분기를 중앙 저장소로 *push*합니다. 개발자가 기능을 게시하기 전에 업데이트된 중앙 커밋을 *fetch*하고 그 위에 변경 사항을 리베이스해야 합니다.

다른 워크플로와 비교하여 중앙 집중식 워크플로에는 정의된 풀 요청 또는 분기 패턴이 없습니다.

###### Source

* https://www.atlassian.com/git/tutorials/comparing-workflows

[[↑] 맨 위로](#Git)
### 로컬 저장소를 업데이트해야 합니다. 어떤 git 명령을 사용할 것인가?

2단계 프로세스입니다. 먼저 원격이라는 이름의 origin에서 변경 사항을 가져옵니다:

```sh
git fetch origin
```
Then you merge a branch master to local:

```sh
git merge origin/master
```
Or simply:

```sh
git pull origin master
```
origin이 기본 원격이고 'master'가 기본 분기인 경우 이를 삭제할 수 있습니다. 'git pull'.

###### Source

* https://samwize.com/2012/10/30/common-git-usage/

[[↑] 맨 위로](#Git)
### 이전 커밋으로 롤백해야 하며 최근 변경 사항은 신경 쓰지 않습니다. 어떤 명령어를 사용해야 할까요?

여러 커밋을 했지만 마지막 몇 개는 잘못되어 이전 커밋으로 롤백하려고 한다고 가정해 보겠습니다:
```sh
git log // lists the commits made in that repository in reverse chronological order
git reset --hard <commit-sha1> // resets the index and working tree
```

###### Source

* https://gist.github.com/chyld/4570933

[[↑] 맨 위로](#Git)
### "git cherry-pick"이란 무엇입니까?

git *cherry-pick* 명령은 일반적으로 저장소 내의 한 분기에서 다른 분기로 특정 커밋을 도입하는 데 사용됩니다. 일반적인 용도는 유지 관리 분기에서 개발 분기로 커밋을 전달 또는 백포트하는 것입니다.

이것은 일반적으로 다른 분기에 많은 커밋을 적용하는 병합 및 리베이스와 같은 다른 방법과 대조됩니다.

Consider:
```sh
git cherry-pick <commit-hash>
```

###### Source

* https://stackoverflow.com/questions/9339429/what-does-cherry-picking-a-commit-with-git-mean

[[↑] 맨 위로](#Git)
### Git에서 작업 트리와 인덱스인 HEAD의 차이점을 알려주세요.

* **working tree/working directory/workspace**는 보고 편집하는 (원본) 파일의 디렉토리 트리입니다.
* **index/staging area**는 <baseOfRepo>/.git/index에 있는 단일 대형 바이너리 파일로, 현재 분기의 모든 파일, sha1 체크섬, 타임스탬프 및 파일 이름이 나열됩니다. 파일 복사본이 포함된 다른 디렉터리가 아닙니다.
* **HEAD**는 현재 체크아웃된 분기의 마지막 커밋에 대한 참조입니다.

###### Source

* https://stackoverflow.com/questions/3689838/whats-the-difference-between-head-working-tree-and-index-in-git

[[↑] 맨 위로](#Git)
### "git stash"는 언제 사용해야 하나요?

`git stash` 명령은 커밋되지 않은 변경 사항(단계적 및 단계적 모두)을 가져와 나중에 사용할 수 있도록 저장한 다음 작업 복사본에서 되돌립니다.

Consider:
```sh
$ git status
On branch master
Changes to be committed:
new file: style.css
Changes not staged for commit:
modified: index.html
$ git stash
Saved working directory and index state WIP on master: 5002d47 our new homepage
HEAD is now at 5002d47 our new homepage
$ git status
On branch master
nothing to commit, working tree clean
```
스태싱을 사용할 수 있는 한 곳은 마지막 커밋에서 무언가를 잊어버렸고 이미 같은 브랜치에서 다음 커밋에서 작업을 시작했다는 것을 발견한 경우입니다:
```sh
# Assume the latest commit was already done
# start working on the next patch, and discovered I was missing something

# stash away the current mess I made
$ git stash save

# some changes in the working dir

# and now add them to the last commit:
$ git add -u
$ git commit --ammend

# back to work!
$ git stash pop
```

###### Source

* https://www.atlassian.com/git/tutorials/saving-changes/git-stash

[[↑] 맨 위로](#Git)
### git에서 이전 커밋을 되돌리는 방법은 무엇입니까?

C는 HEAD이고 (F)는 파일 상태입니다.
```sh
   (F)
A-B-C
    ↑
  master
```
1. 커밋의 변경 사항을 무효화하려면 다음을 수행하십시오:
```sh
git reset --hard HEAD~1
```
이제 B가 HEAD입니다. --hard를 사용했기 때문에 파일이 커밋 B에서 상태로 재설정됩니다.
2. 커밋을 취소하고 변경 사항을 유지하려면 다음을 수행하십시오:
```sh
git reset HEAD~1
```
이제 Git에게 HEAD 포인터를 한 커밋 뒤로 옮기고(B) 파일을 그대로 두도록 지시하고 `git status`는 C에 체크인한 변경 사항을 표시합니다.
3. 커밋을 취소하지만 파일과 인덱스는 그대로 두려면
```sh
git reset --soft HEAD~1
```
`git status`를 실행하면 이전과 동일한 파일이 인덱스에 있는 것을 볼 수 있습니다.

###### Source

* https://stackoverflow.com/questions/927358/how-to-undo-the-most-recent-commits-in-git

[[↑] 맨 위로](#Git)
### Forking Workflow의 장점 설명

**Forking Workflow**는 다른 인기 있는 Git 워크플로와 근본적으로 다릅니다. 단일 서버 측 저장소를 사용하여 "중앙" 코드베이스 역할을 하는 대신 모든 개발자에게 고유한 서버 측 저장소를 제공합니다. Forking Workflow는 공개 오픈 소스 프로젝트에서 가장 자주 볼 수 있습니다.

Forking Workflow의 *주요 장점*은 모든 사람이 깨끗한 프로젝트 기록으로 이어지는 단일 중앙 저장소로 푸시할 필요 없이 기여를 통합할 수 있다는 것입니다. 개발자는 자신의 서버 측 리포지토리로 푸시하고 프로젝트 관리자만 공식 리포지토리로 푸시할 수 있습니다.

개발자가 로컬 커밋을 게시할 준비가 되면 커밋을 공식 저장소가 아닌 자체 공개 저장소에 푸시합니다. 그런 다음 프로젝트 관리자가 업데이트를 통합할 준비가 되었음을 알릴 수 있도록 메인 리포지토리에 풀 요청을 제출합니다.



###### Source

* https://www.atlassian.com/git/tutorials/comparing-workflows/forking-workflow

[[↑] 맨 위로](#Git)
### Gitflow 워크플로를 설명해 주시겠습니까?

Gitflow 워크플로는 두 개의 병렬 *장기 실행* 분기를 사용하여 프로젝트 히스토리 '마스터'와 '개발'을 기록합니다:
* **Master** -  모든 것이 완전히 테스트되고 승인된(프로덕션 준비) 라이브에서 출시될 준비가 되어 있습니다.
 * **Hotfix** -  유지 관리 또는 "핫픽스" 분기를 사용하여 프로덕션 릴리스를 빠르게 패치합니다. 핫픽스 브랜치는 '개발' 대신 '마스터'를 기반으로 한다는 점을 제외하면 릴리스 브랜치 및 기능 브랜치와 매우 유사합니다.


* **Develop** - 모든 기능 분기가 병합되고 모든 테스트가 수행되는 분기입니다. 모든 것을 철저히 확인하고 수정해야만 '마스터'에 병합될 수 있습니다.
 * **Feature** - 각각의 새로운 기능은 자체 분기에 있어야 하며, 상위 분기로 `develop` 분기에 푸시할 수 있습니다.

<div class="text-center">
<img src="https://res.cloudinary.com/practicaldev/image/fetch/s--pLQxGakq--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://wac-cdn.atlassian.com/dam/jcr:61ccc620-5249-4338-be66-94d563f2843c/05%2520%282%29.svg%3FcdnVersion%3Dji" class="img-fluid" style="max-width: 500px;"/>
</div>


###### Source

* https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow

[[↑] 맨 위로](#Git)
### "Rebase Workflow"에 대한 일련의 git 명령을 작성하십시오.

리플레이 변경 사항을 한 작업 라인에서 다른 라인으로 도입된 순서대로 리베이스하는 반면 병합은 끝점을 가져와 함께 병합합니다.

1. feature branch 생성
```sh
$ git checkout -b feature
```
2. feature branch에서 변경
```sh
$ echo "Bam!" >>foo.md
$ git add foo.md
$ git commit -m 'Added awesome comment'
```
3. 업스트림 저장소 가져오기
```sh
$ git fetch upstream
```
4. 기능 분기에서 업스트림/마스터로 변경 사항을 리베이스
```sh
$ git rebase upstream/master
```
5.로컬 마스터를 기능 분기로 리베이스
```sh
$ git checkout master
$ git rebase feature
```
6. 로컬 마스터를 업스트림으로 푸시
```sh
$ git push upstream master
```

Rebasing은 깨끗한 선형 커밋 기록을 제공하고 부지런히 사용하면 프로젝트에 명확하지 않은 이점을 만듭니다. 한 줄의 작업을 수행하고 항상 최신 개정판에서 시작된 척하는 것으로 생각하십시오.

###### Source

* http://kensheedlo.com/essays/why-you-should-use-a-rebase-workflow/

[[↑] 맨 위로](#Git)
### Git에서 "HEAD"는 무엇입니까?

'HEAD'는 현재 체크아웃된 커밋에 대한 ref(참조)입니다.

일반적인 상태에서는 체크아웃한 분기에 대한 심볼적인 참조입니다. .git/HEAD의 내용을 보면 "ref: refs/heads/master"와 같은 것을 볼 수 있습니다. 분기 자체는 분기 끝에 있는 커밋에 대한 참조입니다. 따라서 정상 상태에서 HEAD는 효과적으로 현재 분기 끝에 있는 커밋을 나타냅니다.

Detached HEAD를 갖는 것도 가능하다. 원격 분기, 특정 커밋 또는 태그와 같은 (로컬) 분기 이외의 항목을 체크 아웃할 때 이 문제가 발생합니다. 이러한 상황을 가장 일반적으로 확인할 수 있는 위치는 커밋을 편집하도록 선택한 대화형 기본 재배치 중에 나타납니다. 분리된 HEAD 상태에서 HEAD는 커밋에 대한 직접적인 참조이며 .git/HEAD의 내용은 SHA1 해시가 됩니다.

일반적으로 HEAD는 "체크아웃한 항목"을 의미하는 편리한 이름일 뿐이므로 크게 걱정할 필요가 없습니다. 체크아웃한 내용을 숙지하고, 현재 수행 중인 작업(예: 대화형 리베이스에 있음)을 알지 못하는 한 분기(분리된 HEAD 상태)에 있지 않은 경우 커밋하고 싶지 않을 수 있음을 기억하십시오. 

###### Source

* https://stackoverflow.com/questions/2529971/what-is-the-head-in-git

[[↑] 맨 위로](#Git)
### 파일 시스템에서 파일을 제거하지 않고 git에서 파일을 제거하는 방법은 무엇입니까?

`git add`를 할 때 주의하지 않으면 커밋하고 싶지 않은 파일이 추가될 수 있습니다. 그러나 `git rm`은 스테이징 영역(색인)과 파일 시스템(작업 트리) 모두에서 제거할 것이므로 원하지 않을 수 있습니다.

대신 `git reset`을 사용하세요:
```sh
git reset filename          # or
echo filename >> .gitingore # add it to .gitignore to avoid re-adding it
```

이것은 `git reset <paths>`가 `git add <paths>`의 반대임을 의미합니다.

###### Source

* https://www.codementor.io/citizen428/git-tutorial-10-common-git-problems-and-how-to-fix-them-aajv0katd

[[↑] 맨 위로](#Git)
### "git stash pop"과 "git stash apply"의 차이점은 무엇입니까?

`git stash pop`은 적용한 후 (기본적으로 최상위) stash를 **던집니다** 반면 `git stash apply`는 나중에 재사용할 수 있도록 **stash 목록에 남겨둡니다**. stash drop` it).

이것은 `git stash pop` 이후에 충돌이 발생하지 않는 한 발생합니다(예를 들어 stash를 처음 생성한 이후에 수행한 다른 변경 사항과 stash된 변경 사항이 충돌한다고 가정). 이 경우 `git stash와 똑같이 작동하여 stash를 제거하지 않습니다. 숨김 적용`.

그것을 보는 또 다른 방법: `git stash pop`은 `git stash apply && git stash drop`입니다.

###### Source

* https://stackoverflow.com/questions/15286075/difference-between-git-stash-pop-and-git-stash-apply

[[↑] 맨 위로](#Git)
### "git reset"이 일반 영어로 무엇을 하는지 설명할 수 있습니까?

일반적으로 `git reset` 기능은 현재 분기를 가져와 다른 곳을 가리키도록 재설정하고 인덱스와 작업 트리를 함께 가져오는 것입니다.

```sh
- A - B - C (HEAD, master)
# after git reset B (--mixed by default)
- A - B (HEAD, master)      # - C is still here (working tree didn't change state), but there's no branch pointing to it anymore
```

git에 다음이 있음을 기억하십시오:
* 작업 중인 커밋을 알려주는 HEAD 포인터
* 시스템의 파일 상태를 나타내는 작업 트리
* 나중에 함께 커밋될 수 있도록 "단계"가 변경되는 준비 영역(색인이라고도 함)

So consider:
* `git reset --soft`는 HEAD를 이동하지만 스테이징 영역이나 작업 트리는 건드리지 않습니다.
* `git reset --mixed`는 HEAD를 이동하고 스테이징 영역을 업데이트하지만 작업 트리는 업데이트하지 않습니다.
* `git reset --merge`는 HEAD를 이동하고 스테이징 영역을 재설정하며 작업 트리의 모든 변경 사항을 새 작업 트리로 이동하려고 시도합니다.
* `git reset --hard`는 HEAD를 이동하고 스테이징 영역과 작업 트리를 새 HEAD로 조정하여 모든 것을 버립니다.

Use cases:
* "losing your place" 다른 커밋으로 이동하고 패치를 적용하려면 `--soft`를 사용하세요. 이것이 필요한 경우는 매우 드뭅니다.
* 다른 커밋에서 어떻게 보이는지 보고 싶지만 이미 있는 변경 사항을 잃지 않으려면 `--mixed`(기본값)를 사용하십시오.
* 새로운 지점으로 이동하고 싶지만 작업 트리에 이미 있는 변경 사항을 통합하려면 `--merge`를 사용하세요.
* `--hard`를 사용하여 모든 것을 지우고 새 커밋에서 새 슬레이트를 시작합니다.

###### Source

* https://stackoverflow.com/questions/2530060/can-you-explain-what-git-reset-does-in-plain-english

[[↑] 맨 위로](#Git)
### 두 커밋의 차이점을 확인하기 위해 git 명령을 작성하십시오.

`git diff`를 사용하면 분기 또는 커밋 간의 차이점을 확인할 수 있습니다. 자동으로 입력하면 마지막 커밋과 현재 변경 사항 간의 차이점을 확인할 수 있습니다.

```sh
git diff <branch_or_commit_name> <second_branch_or_commit>
```



[[↑] 맨 위로](#Git)
### 이전 Git 커밋을 수정하는 방법은 무엇입니까?

```sh
git rebase -i HEAD^^^
```
이제 수정하려는 항목을 'edit' 또는 'e'로 표시합니다('pick' 대체). 이제 저장하고 종료합니다.

이제 내용을 변경합니다:
```sh
git add -A
git commit --amend --no-edit
git rebase --continue
```
추가 삭제를 추가하려면 커밋 명령에서 옵션을 제거하십시오. 메시지를 조정하려면 `--no-edit` 옵션만 생략합니다.

###### Source

* https://stackoverflow.com/questions/8824971/how-to-amend-older-git-commit/18150592#18150592

[[↑] 맨 위로](#Git)
### 특정 파일의 특정 줄을 누가 변경했는지 알기 위해 어떤 git 명령을 사용해야 합니까?

저장소에 누가 무엇을 썼는지 볼 수 있는 git의 작은 기능인 `git 비난`을 사용하세요. 특정 행을 변경한 사람을 알고 싶다면 -L 플래그를 사용하여 해당 행을 변경한 사람을 파악할 수 있습니다. 다음 명령을 사용할 수 있습니다:
```sh
git blame -L <line-number>,<ending-linenumber> <filename>
```

###### Source

* https://github.com/mikeizbicki/ucr-cs100/tree/2015winter/textbook/tools/git/advanced-git

[[↑] 맨 위로](#Git)
### "git merge" 대신 "git rebase"를 언제 사용합니까?

이 두 명령은 모두 한 분기에서 다른 분기로 변경 사항을 통합하도록 설계되었습니다. 단지 매우 다른 방식으로 수행할 뿐입니다.

병합/리베이스 전에 다음 사항을 고려하십시오:
```js
A <- B <- C    [master]
^
 \
  D <- E       [branch]
```
`git merge master` 후:
```js
A <- B <- C
^         ^
 \         \
  D <- E <- F
```
`git rebase master` 후:
```js
A <- B <- C <- D <- E
```

rebase를 사용하면 다른 분기를 작업의 새 기반으로 사용한다고 말합니다.

**사용 시기:**
1. 의심이 가는 경우 merge를 사용합니다.
2. 히스토리가 어떻게 생겼는지에 따라 rebase 또는 merge를 선택합니다.

**고려할 추가 요소:**
1. **변경 사항을 받고 있는 브랜치가 팀 외부의 다른 개발자(예: 오픈 소스, 공개)와 공유됩니까?** 그렇다면 리베이스하지 마십시오. Rebase는 분기를 파괴하고 해당 개발자는 `git pull --rebase`를 사용하지 않는 한 손상되거나 일관성이 없는 리포지토리를 갖게 됩니다.
2. **개발팀의 숙련도는 어느 정도입니까?** Rebase는 파괴적인 작업입니다. 즉, 올바르게 적용하지 않으면 커밋된 작업이 손실되거나 다른 개발자 저장소의 일관성이 깨질 수 있습니다.
3. **분기 자체가 유용한 정보를 나타내는가?** 일부 팀은 각 분기가 기능(또는 버그 수정, 하위 기능 등)을 나타내는 *기능별 분기* 모델을 사용합니다. 이 모델에서 분기가 도움이 됩니다. 관련된 커밋 세트를 식별합니다. *branch-per-developer* 모델의 경우 분기 자체는 추가 정보를 전달하지 않습니다(커밋에 이미 작성자가 있음). 리베이스에 해가 없을 것입니다.
4. **어떤 이유로든 병합을 되돌리고 싶으십니까?** 병합을 되돌리는 것과 비교하여 rebase(리베이스에 충돌이 있는 경우)를 되돌리는 것은 상당히 어렵거나 불가능합니다. 되돌릴 가능성이 있다고 생각되면 병합을 사용하십시오.


###### Source

* https://stackoverflow.com/questions/804115/when-do-you-use-git-rebase-instead-of-git-merge

[[↑] 맨 위로](#Git)
### git rebase를 쉽게 취소하는 방법을 알고 있습니까?

가장 쉬운 방법은 `reflog`에서 rebase가 시작되기 직전에 있던 브랜치의 헤드 커밋을 찾는 것입니다.

```git
git reflog
```
그리고 현재 분기를 그것으로 재설정하기 위해 (`--hard` 옵션으로 재설정하기 전에 절대적으로 확신해야 한다는 일반적인 주의사항과 함께).

이전 커밋이 ref 로그에서 `HEAD@{5}`라고 가정합니다.
```git
git reset --hard HEAD@{5}
```

또한 rebase는 시작점을 `ORIG_HEAD`에 저장하므로 일반적으로 다음과 같이 간단합니다.
```git
git reset --hard ORIG_HEAD
```


###### Source

* https://stackoverflow.com/questions/134882/undoing-a-git-rebase

[[↑] 맨 위로](#Git)
