# 소개
- test_amr_emulator는 차량없이 FMS-AMR의 연결테스트를 가능하게 함
- 
<mark>highlighted text</mark>.
# 사용법
- Terminal 실행
- mqtt 서버주소 설정
  - server_address: "tcp://localhost:1883"
```
./test_amr_emulator/config/amr_params.yaml

[amr_params.yaml]
amr_count: 1
:
:
:
mqtt:
  server_address: "tcp://localhost:1883"
```
- emulator 실행
./run.sh

# 통신 시퀀스





