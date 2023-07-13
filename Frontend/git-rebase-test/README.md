## Git Command

- `git rebase [-i]`
    - commit 이력 수정
    - 첫번째만 pick 으로 설정하고 나머지는 squash(s)로 하여 한개의 커밋만 유지

- `git rebase --abort`
    - rebase 진행하기 전 상황으로 돌아감

- `git rebase --continue`
    - rebase를 하다가 충돌이 나면 rebase가 중단되기 때문에 `git rebase --continue`를 하여 rebase를 계속 진행하게 만든다.

- `git reflog`
    - 로컬 저장소에서 HEAD의 업데이트를 기록을 출력. 업데이트의 내용은 저장소 디렉토리의 `.git/logs/refs/heads/. `혹은 `.git/logs/HEAD`에 기록되며 git reflog는 이 내용을 출력

- `git reset`
    - commit 취소를 할 수 있는 명령어 reflog로 취소하고 싶은 hash id를 확인한 후 `git reset --hard [hash id값]`을 명령한다.
