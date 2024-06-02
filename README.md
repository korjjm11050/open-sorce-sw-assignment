# open-sorce-sw-assignment
assinment repository

___

## 1. `top` 명령어
- **설명**:
`top` 명령어는 실시간으로 시스템에서 실행 중인 프로세스의 목록을 보여줍니다. CPU 및 메모리 사용량, 실행 시간 등 다양한 정보를 제공합니다.

![TOP](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FddHQnx%2FbtqEFEw62PN%2F0kcwA8LSu0rpqL15oKURqK%2Fimg.png)

- **옵션**:

|옵션|설명|
|-------------|--------------|
|top -c | 프로세스의 전체경로를 표기함, 정확한 정보 확인 가능|
|top -d 1 | 1초 간격으로 새로 고침|
|top 실행 후 Shift + p |  각 프로세스들의 CPU 사용률이 높은 순서대로 정렬|
|top 실행후 shift + m | 각 프로세스들의 memory 사용량이 가장 많은 순서대로 정렬|
|top 실행후 숫자 1| cpu 별 이용률 보여줌|
|top 실행후 u 입력, 유저이름 입력 | 특정 유저가 실행시킨 process확인|
|top 실행후 k 입력,| PID 입력 특정 프로세스를 종료할때 사용|


## 2. `ps` 명령어
`ps` 명령어는 현재 실행 중인 프로세스의 스냅샷을 보여줍니다. `ps`는 실시간으로 업데이트되지 않으며, 특정 시점의 프로세스 상태를 보여줍니다.

![PS -A](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2Fbv7axc%2FbtqED1UuhSy%2FyATfSkCgvuFbI6opBYNlkK%2Fimg.png)

- **주요 옵션**:
- 
|옵션|설명|
|--------------|-----------------|
|ps -A	|모든 프로세스를 출력|
|ps -a	|세션 리더을 제외하고 데몬 프로세스처럼 터미널에 종속되지 않은 모든 프로세스를 출력|
|ps -e	|커널 프로세스를 제외한 모든 프로세스를 출력(UID, PID, PPID등이 함께 표시)|
|ps -f	|full 포맷 출력 |
|ps -l	|긴 포맷으로 출력(프로세스의 정보를 길게 보여주는 옵션으로 우선순위와 관련된 PRI와 NI값을 확인 가능)|
|ps -o| 값	출력 포맷을 지정하는 옵션으로 값으로는 pid, tty, time, cmd 등을 지정하여 출력|
|ps -M	|64비트 프로세스 출력|
|ps -m	|프로세스들 뿐만 아니라 커널 스레드들 출력|
|ps -p	|특정 PID를 지정할 때 사용|
|ps -r	|현재 실행 중인 프로세서를 출력|
|ps u	|프로세스의 소유자를 기준으로 출력|
|ps x	|특정 사용자의 프로세스 정보를 확인할 때 사용,사용자를 지정하지 않으면 현재 사용자를 기준으로 정보를 출력|
|ps -x	|로그인 상태에 있는 동안 아직 완료되지 않은 프로세서들을 출력|

## 3. `jobs` 명령어
`jobs` 명령어는 현재 셸 세션에서 실행 중인 백그라운드 및 포어그라운드 작업의 목록을 표시합니다.

![PS -A](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FBviAe%2FbtqZpT84ElO%2FwEuAaRkktUJq5XiGUcZ8X0%2Fimg.png)

- **주요 옵션**:
|l 옵션| 프로세스 ID와 함께 잡 목록을 출력합니다.|
|n 옵션| 마지막로 알림 이후 변경된 잡만 출력합니다.|
|p 옵션| 잡의 프로세스 ID만 출력합니다.|
|r 옵션| 실행 중인 잡만 출력합니다.|
|s 옵션| 중지된 잡만 출력합니다.|

## 4. `kill` 명령어
`kill` 명령어는 특정 프로세스를 종료하는 데 사용됩니다. 주로 `ps`나 `top` 명령어로 PID를 확인한 후, 해당 PID를 사용하여 프로세스를 종료합니다.

![PS -A](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2Fbv7axc%2FbtqED1UuhSy%2FyATfSkCgvuFbI6opBYNlkK%2Fimg.png)


- **주요 옵션**:
| 옵션 | 설명 |
  |---|---|
  | `kill -9 PID` | 강제 종료(SIGKILL) |
  | `kill -l` | 사용 가능한 모든 시그널의 목록을 표시 |
  | `kill -s <signal> PID` | 특정 시그널을 지정하여 프로세스를 종료 (예: `kill -s SIGTERM PID`) |

## 5.출처

1.[top](https://jang8584.tistory.com/198)
2.[ps](https://blog.naver.com/tmk0429/222318530824)
3.[jobs](https://codingfarm.tistory.com/449)
4.[kill](https://bigsun84.tistory.com/355)













