# 소개
- test_amr_emulator는 차량없이 FMS-AMR의 연결테스트를 가능하게 함

# 사용법
- Terminal 실행
- mqtt 서버주소 설정
  - server_address 수정
  - server_address: "tcp://localhost:1883"
```
./test_amr_emulator/config/amr_params.yaml

[amr_params.yaml]
amr_count: 1
base_port: 8080
speedup_ratio: 10
protocol_type: "vda5050"
vehicle_type : "steering_drive"   #"differential_drive"
:
:
:
battery_params:
  idle_discharge_per_sec: 0.001 # 유휴기간 0.001%, 정지상태 28시간 후 0% 방전
  max_charge_per_sec: 0.01  # 약 100% 충전소요시간 : 2시간 45분
  charge_stop_threshold: 90.0 # 충전제한 : 90%
  linear_slope: 0.004
  angular_slope: 0.002
  acceleration_factor: 0.001
mqtt:
  server_address: "tcp://localhost:1883"
- emulator 실행


```
./run.sh




