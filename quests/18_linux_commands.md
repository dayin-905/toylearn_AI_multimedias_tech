## 🧠 Linux 명령어 연습 문제
## 문제 1
~/commands 폴더로 이동한 뒤, 현재 작업 위치를 확인하세요.
💡 힌트: cd 명령어와 pwd 명령어를 함께 사용합니다.
```
~ $ cd Commands/ && pwd && ls -l
/home/node/Commands
total 0
-rw-r--r--    1 node     node             0 Nov  7 03:07 temp_01.txt
```


## 문제 2
~/commands 폴더 안에 test라는 새 폴더를 만들고, 폴더 목록을 확인하세요.
💡 힌트: mkdir와 ls를 함께 사용합니다.
```
~/Commands $ mkdir test && ls -l
total 4
-rw-r--r--    1 node     node             0 Nov  7 03:07 temp_01.txt
drwxr-sr-x    2 node     node          4096 Nov  7 03:43 test
```

## 문제 3
~/commands 안에 notes 폴더를 만든 뒤, 해당 폴더로 이동하고 현재 위치를 확인하세요.
💡 힌트: mkdir, cd, pwd 순으로 실행합니다.
```
~/Commands $ mkdir notes && cd notes && pwd
/home/node/Commands/notes
~/Commands/notes $ 
```

## 문제 4
~/commands 폴더 안에 images, videos, docs 세 개의 폴더를 한 번에 만들고, 생성된 폴더들을 확인하세요.
💡 힌트: mkdir images videos docs 또는 mkdir -p images videos docs
```
~/Commands $ mkdir -p images videos docs && pwd && ls -l
/home/node/Commands
total 20
drwxr-sr-x    2 node     node          4096 Nov  7 03:45 docs
drwxr-sr-x    2 node     node          4096 Nov  7 03:45 images
drwxr-sr-x    2 node     node          4096 Nov  7 03:44 notes
-rw-r--r--    1 node     node             0 Nov  7 03:07 temp_01.txt
drwxr-sr-x    2 node     node          4096 Nov  7 03:43 test
drwxr-sr-x    2 node     node          4096 Nov  7 03:45 videos
```

## 문제 5
~/commands 안의 docs 폴더로 이동한 뒤, 상위 폴더(~/commands)로 돌아가서 폴더 목록을 다시 확인하세요.
💡 힌트: cd docs, cd .., ls
```
~/Commands $ cd docs/
~/Commands/docs $ cd ../
~/Commands $ ls
docs         images       notes        temp_01.txt  test         videos
```