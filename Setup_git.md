# Setup Git

## Daily setup

1. pull main branch

   ```git
   git pull origin main
   ```

   main branch 에서 일단 data update

2. create branch

   ```git
   git checkout -b dev_<날짜명>
   ```

   나중에 Pull Request 동작으로 오늘 개발 전체를 올릴 예정

3. add / commit

	```git
	git add <file 명>
	git commit -m "message content"
	```

	file 명에 . 이용시 현재 폴더 전체를 의미.
	
4. push

   ```git
   git push origin dev_<날짜명>
   ```

   가능한 한번에 push 하자

   그리고 github에서 마무리 Pull Request 정리하면 하루 끝



## Add 및 Commit 취소

`git log`를 통해서 log 기록을 확인

`git reset --hard <HEAD number>` 해당 CMD를 이용해 현재 위치를 변경
Conflict 또한 이와 같은 것으로 복귀할 수 있다.

cf) `git reset --soft` 도 있다. revert histroy를 남기기 위해



`git commit -amend "message"` 를 통해서 마지막 commit의 내용을 바꿀 수 있다.
해당 Commend 전에 add를 하여 파일 수정 사항이나 삭제 추가도 할 수 있다.