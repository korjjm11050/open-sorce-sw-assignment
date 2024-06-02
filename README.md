# open-sorce-sw-assignment
assinment repository

___

## 1. `top` 명령어
`top` 명령어는 실시간으로 시스템에서 실행 중인 프로세스의 목록을 보여줍니다. CPU 및 메모리 사용량, 실행 시간 등 다양한 정보를 제공합니다.

![image](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FddHQnx%2FbtqEFEw62PN%2F0kcwA8LSu0rpqL15oKURqK%2Fimg.png)

- **옵션**:

|제목|내용|설명|
|------|---|---|
|테스트1|테스트2|테스트3|
|테스트1|테스트2|테스트3|
|테스트1|테스트2|테스트3|




|옵션|설명|

|_______________|____________|

|top -c :| 프로세스의 전체경로를 표기함, 정확한 정보 확인 가능|

|top -d 1 :| 1초 간격으로 새로 고침|

|top 실행 후 Shift + p :|  각 프로세스들의 CPU 사용률이 높은 순서대로 정렬|

|top 실행후 shift + m :| 각 프로세스들의 memory 사용량이 가장 많은 순서대로 정렬|

|top 실행후 숫자 1 :| cpu 별 이용률 보여줌|

|top 실행후 u 입력, 유저이름 입력 :| 특정 유저가 실행시킨 process확인|

|top 실행후 k 입력,| PID 입력 특정 프로세스를 종료할때 사용|


## 2. `ps` 명령어
`ps` 명령어는 현재 실행 중인 프로세스의 스냅샷을 보여줍니다. `ps`는 실시간으로 업데이트되지 않으며, 특정 시점의 프로세스 상태를 보여줍니다.

- **사용법**: 터미널에서 `ps`를 입력하고 엔터 키를 누릅니다.
- **주요 옵션**:
  - `aux` : 모든 사용자의 모든 프로세스를 상세하게 표시합니다. 예: `ps aux`.
  - `-e` : 모든 프로세스를 표시합니다. 예: `ps -e`.
  - `-f` : 풀 포맷으로 표시합니다. 예: `ps -ef`.
  - `-u` : 특정 사용자의 프로세스만 표시합니다. 예: `ps -u username`.

## 3. `jobs` 명령어
`jobs` 명령어는 현재 셸 세션에서 실행 중인 백그라운드 및 포어그라운드 작업의 목록을 표시합니다.

- **사용법**: 터미널에서 `jobs`를 입력하고 엔터 키를 누릅니다.
- **주요 옵션**:
  - `-l` : 각 작업에 대한 프로세스 ID (PID)를 포함하여 상세하게 표시합니다.
  - `-p` : 각 작업의 프로세스 ID만 표시합니다.

## 4. `kill` 명령어
`kill` 명령어는 특정 프로세스를 종료하는 데 사용됩니다. 주로 `ps`나 `top` 명령어로 PID를 확인한 후, 해당 PID를 사용하여 프로세스를 종료합니다.

- **사용법**: 터미널에서 `kill PID`를 입력하고 엔터 키를 누릅니다.
- **주요 옵션**:
  - `-9` : 강제 종료(SIGKILL)합니다. 예: `kill -9 PID`.
  - `-l` : 사용 가능한 모든 시그널의 목록을 표시합니다.
  - `-s` : 특정 시그널을 지정하여 프로세스를 종료합니다. 예: `kill -s SIGTERM PID`.

각 명령어는 시스템의 프로세스 관리에 매우 유용하며, 다양한 옵션을 제공하여 사용자가 필요에 맞게 프로세스를 모니터링하고 제어할 수 있게 합니다.
