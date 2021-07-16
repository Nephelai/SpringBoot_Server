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
