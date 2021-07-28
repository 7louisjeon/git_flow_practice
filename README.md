git flow init

git branch

gir flow feature start helloworld

git branch

touch hello.py

vi hello.py (write commands)

cat hello.py

git status

git add hello.py

git commit (feat: Create hello.py)

git branch

git flow feature finish helloworld

git branch

git flow release start v0.1

git flow rlease finish v0.1

:wq (main으로 merge하는 커밋)

패치노트 작성 후 :wq 

:wq (develop으로 merge하는 커밋)

git push -u origin develop (local repo에서 develop branch로 push)

git checkout main

git push origin main

git tag (tag 확인)

git push --tags (tags push)

git branch

git checkout develop

파일 이동이 필요하거나 이름을 바꿔야 할 때 그냥 mv를 사용하면 새로운 파일이 생성된 것으로 간주하여 위험함
git mv를 이용 (git mv hello.py world.py) (기록을 남기는 관점에서 정확함 / git을 왜 쓰는지에 대한 철학적 고찰)

README.md를 변경한 후 git restore README.md를 통해 이전 단계로 복원 가능

git reset HEAD world.py를 통해 stage에 올라갔던 (add .) 파일들 중 world.py를 unstage할 수 있다.

commit은 제거할 수는 없지만 특정 커밋으로 되돌아가 다시 시작하는것은 가능

git commit --amend: push하기 전에 방금 전 한 커밋을 수정할 수 있음

git log로 log check가능

RESET: 아예 커밋을 지움 / 흔적도 남기지 않음

REVERT: 몇 단계 전으로 돌아가고 기록을 남김

git revert --no-commit HEAD~3.. : 지금 시점에서 3단계의 commit을 되돌림 (3이 없으면 한단계) (--no-commit: commit을 한단계 쓰겟다)
