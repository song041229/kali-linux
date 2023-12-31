# tmux

### 1. Theory ###
  - 여러 터미널을 독립적인 환경에서 실행
  - 프로그램 분리에 유용

### 2. Download ###
  ```
  sudo apt-get install tmux
  ```
  - 참고 : 일반적으로 내장되어 있음

### 3. Command ###

1. Session
  ```
  # 새로운 세션 생성 (default : 숫자)
  $ tmux

  # 이름을 지정하여 세션 생성
  $ tmux new -s <name>


  # 현재 세션 list
  $ tumx ls

  # 특정 이름인 세션으로 돌아가기
  $ tumx a -t <name>
  ```

2. Window
  ```
  # 새로운 윈도우 생성
  $ ctrl+b, c

  # 현재 윈도우 닫기
  $ ctrl+d


  # 특정 이름을 가진 윈도우로 이동
  $ ctrl + b, f -> <name>

  # 이전 윈도우로 이동
  $ ctrl+b, p

  # 다음 윈도우로 이동
  $ ctrl+b, n 


  # 현재 윈도우 이름 바꾸기
  $ ctrl+b, ,


  # 현재 윈도우 목록 나열
  $ ctrl+b, w 
  ```

3. Pane
  ```
  # 화면을 세로로 분할
  $ ctrl+b, %

  # 화면을 가로로 분할
  $ ctrl+b, "

  # pane 옮겨 다니기
  $ ctrl+b, <arrow>
  ```

4. Extra
  ```
  # 세션 종료
  $ exit

  # 세션 종료
  $ tmux kill-session -t <name>
  ```
