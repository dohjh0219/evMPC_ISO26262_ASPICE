# System Requirements Specification (SYS.2)

## 1. Item Definition
본 시스템은 4륜 독립 구동 전기차(In-Wheel Motor EV)를 위한 토크 벡터링 제어기이다.
운전자의 조향 의도와 차량의 실제 거동 차이를 최소화하여 선회 안정성을 확보한다.

## 2. Functional Requirements
| Req ID | Category | Description | Performance Criteria | ASIL |
| :--- | :--- | :--- | :--- | :--- |
| **SYS-REQ-001** | Control | 요레이트(Yaw Rate) 추종 제어 | 목표값 대비 오차 **5% 이내** 유지 | B |
| **SYS-REQ-002** | Safety | 휠 슬립(Wheel Slip) 방지 | 슬립율(Slip Ratio) **0.2 이하** 유지 | B |
| **SYS-REQ-003** | Interface | CAN 통신 주기 준수 | 제어 주기 **10ms (100Hz)** 보장 | QM |
| **SYS-REQ-004** | Fail-Safe | 센서 고장 감지 | IMU 센서 미수신 시 **Safe Mode(토크 0)** 진입 | C |