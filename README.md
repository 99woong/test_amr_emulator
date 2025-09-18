# 소개
- test_amr_emulator는 차량없이 FMS-AMR의 연결테스트를 가능하게 함
# 사용법
- Terminal 실행
- mqtt server 파라메터(amr_params.yaml) 수정
```
$vim ~/test_amr_emulator/config/amr_params.yaml

[amr_params.yaml]
amr_count: 1
:
:
:
mqtt:
  server_address: "tcp://localhost:1883"
```

- emulator 실행
$./run.sh

# 통신 시퀀스





