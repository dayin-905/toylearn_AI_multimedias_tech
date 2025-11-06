### commands 폴더 생성
```
PS C:\Users\PC> cd ../
PS C:\Users> cd ../
PS C:\> cd ../
PS C:\> mkdir commands


    디렉터리: C:\


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----      2025-11-06   오후 5:45                commands

```
### ① 폴더 이동 후 현재 위치 확인
```
PS C:\> cd C:\Commands
PS C:\Commands> pwd

Path
----
C:\Commands


PS C:\Commands>
```

### ② 새 폴더 생성 후 목록 확인
```
PS C:\Commands> mkdir Projects


    디렉터리: C:\Commands


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----      2025-11-06   오후 5:48                Projects


PS C:\Commands> ls


    디렉터리: C:\Commands


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----      2025-11-06   오후 5:48                Projects

```

### ③ 하위 폴더 생성 후 이동 및 현재 위치 확인
```
PS C:\commands> mkdir Logs


    디렉터리: C:\commands


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----      2025-11-06   오후 5:49                Logs


PS C:\commands> cd .\Logs\
PS C:\commands\Logs> pwd

Path
----
C:\commands\Logs

```

### ④ 여러 개의 폴더를 차례로 만들고 목록 출력
```
PS C:\commands\Logs> cd ../
PS C:\commands> mkdir Data, Reports, Backup


    디렉터리: C:\commands


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----      2025-11-06   오후 5:50                Data
d-----      2025-11-06   오후 5:50                Reports
d-----      2025-11-06   오후 5:50                Backup


PS C:\commands> ls


    디렉터리: C:\commands


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----      2025-11-06   오후 5:50                Backup
d-----      2025-11-06   오후 5:50                Data
d-----      2025-11-06   오후 5:49                Logs
d-----      2025-11-06   오후 5:48                Projects
d-----      2025-11-06   오후 5:50                Reports

```

### ⑤ 특정 폴더로 이동한 뒤 상위 폴더 목록 확인
```
PS C:\commands> cd .\Backup\
PS C:\commands\Backup> cd ..
PS C:\commands> ls


    디렉터리: C:\commands


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----      2025-11-06   오후 5:50                Backup
d-----      2025-11-06   오후 5:50                Data
d-----      2025-11-06   오후 5:49                Logs
d-----      2025-11-06   오후 5:48                Projects
d-----      2025-11-06   오후 5:50                Reports

```

## PowerShell 명령 연습 문제
### 문제 1
C:\Commands 폴더로 이동한 뒤, 현재 작업 위치를 확인하세요.
```
PS C:\commands> pwd

Path
----
C:\commands

```
### 문제 2
 C:\Commands 폴더 안에 Test라는 새 폴더를 만들고, 폴더 목록을 확인하세요.
 ```
 PS C:\commands> mkdir Test


    디렉터리: C:\commands


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----      2025-11-06   오후 5:57                Test


PS C:\commands> cd .\Test\
PS C:\commands\Test> ls
 ```
### 문제 3
 C:\Commands 안에 Notes 폴더를 만든 뒤, 해당 폴더로 이동하고 현재 위치를 확인하세요
 ```
PS C:\commands\Test> cd ..
PS C:\commands> mkdir Notes


    디렉터리: C:\commands


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----      2025-11-06   오후 5:54                Notes


PS C:\commands> cd notes
PS C:\commands\notes> pwd

Path
----
C:\commands\notes


 ```

### 문제 4
 C:\Commands 폴더 안에 Images, Videos, Docs 세 개의 폴더를 한 번에 만들고, 생성된 폴더들을 확인하세요.
```
PS C:\commands> mkdir Images, Videos, Docs


    디렉터리: C:\commands


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----      2025-11-06   오후 5:55                Images
d-----      2025-11-06   오후 5:55                Videos
d-----      2025-11-06   오후 5:55                Docs


PS C:\commands> ls


    디렉터리: C:\commands


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----      2025-11-06   오후 5:50                Backup
d-----      2025-11-06   오후 5:50                Data
d-----      2025-11-06   오후 5:55                Docs
d-----      2025-11-06   오후 5:55                Images
d-----      2025-11-06   오후 5:49                Logs
d-----      2025-11-06   오후 5:54                Notes
d-----      2025-11-06   오후 5:48                Projects
d-----      2025-11-06   오후 5:50                Reports
d-----      2025-11-06   오후 5:53                Test
d-----      2025-11-06   오후 5:55                Videos


```

### 문제 5
C:\Commands 안의 Docs 폴더로 이동한 뒤, 상위 폴더(C:\Commands)로 돌아가서 폴더 목록을 다시 확인하세요.
```
PS C:\commands> cd .\Docs\
PS C:\commands\Docs> cd ..
PS C:\commands> ls


    디렉터리: C:\commands


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----      2025-11-06   오후 5:50                Backup
d-----      2025-11-06   오후 5:50                Data
d-----      2025-11-06   오후 5:55                Docs
d-----      2025-11-06   오후 5:55                Images
d-----      2025-11-06   오후 5:49                Logs
d-----      2025-11-06   오후 5:54                Notes
d-----      2025-11-06   오후 5:48                Projects
d-----      2025-11-06   오후 5:50                Reports
d-----      2025-11-06   오후 5:53                Test
d-----      2025-11-06   오후 5:55                Videos


```