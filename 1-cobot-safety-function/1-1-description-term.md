# 1.1 용어 설명

### <mark style="color:green;">로봇 제한 파라미터</mark>&#xD;

로봇의 속도, 힘 운동량을 감시하기 위해 기준이 되는 파라미터입니다.

*   **TCP 위치 감시**

    안전 툴 모델이 안전 영역을 위반하는지 감시. 영역을 침범하는 경우 사용자가 설정한 안전 정지 수행
*   **TCP 방향 감시**

    툴의 방향이 지정된 범위를 벗어나지 않는지 감시. 기준값을 초과하는 경우 사용자가 설정한 안전 정지 수행
*   **TCP 속도 감시**

    툴 끝의 속도를 감시. 기준값을 초과하는 경우 사용자가 설정한 안전 정지 수행
*   **TCP 힘 감시**

    툴 끝의 힘을 감시. 기준값을 초과하는 경우 사용자가 설정한 안전 정지 수행
*   **파워 감시**

    로봇의 파워를 감시. 기준값을 초과하는 경우 사용자가 설정한 안전 정지 수행
*   **모멘텀 감시**

    로봇의 모멘텀을 감시. 기준값을 초과하는 경우 사용자가 설정한 안전 정지 수행
*   **충돌 검지**

    로봇에 외력이 가해져 허용치를 초과하는 경우 사용자가 설정한 안전 정지 수행
*   **안전 정지 감시(SOS, Safe Operating Stop)**

    로봇이 슬립 발생 없이 정지 상태를 유지하는지 감시. 기준값을 초과하는 경우 정지0을 수행. 자동 모드에서 정지 상태가 되면 기능이 자동으로 동작

### <mark style="color:green;">조인트 제한 파라미터</mark>&#xD;

로봇 각 조인트의 위치, 속도, 토크를 감시하기 위해 기준이 되는 파라미터입니다.

*   **조인트 각도 감시**

    각 축 조인트의 위치를 감시. 기준값을 초과하는 경우 사용자가 설정한 안전 정지 수행
*   **조인트 속도 감시**

    각 축 조인트의 속도를 감시. 기준값을 초과하는 경우 사용자가 설정한 안전 정지 수행
*   **조인트 토크 감시**

    각 축 조인트의 토크를 감시. 기준값을 초과하는 경우 사용자가 설정한 안전 정지 수행



### <mark style="color:green;">안전 레이아웃</mark>&#xD;

TCP 위치와 방향 감시를 위해 기준이 되는 안전 영역과 툴 영역의 파라미터입니다.

*   **안전 영역**

    툴의 작업 영역과 보호 영역의 통칭
*   **작업 영역**

    로봇이 작업을 수행하는 영역. 툴 및 로봇 엘보우 모델이 작업 영역을 벗어나는 경우 안전 정지 수행
*   **보호 영역**

    로봇으로부터 보호되어야 하는 영역. 툴 및 로봇 엘보우 모델이 보호 영역을 침범하는 경우 안전 정지 수행
*   **안전 툴 모델링**

    TCP 위치와 방향 감시를 위해 로봇에 부착된 툴을 구와 원뿔로 모델링
*   **안전 로봇 모델링**

    로봇 엘보우를 구로 모델링하여 안전 영역과의 거리를 감시



### <mark style="color:green;">안전 정지</mark>&#xD;

안전에 위반이 되는 경우 안전한 상태로 만들기 위해 로봇을 정지시키는 것으로 정지 방법에는 3 가지가 있습니다. 각 정지 방법에 대한 자세한 정보는 “ISO 13850” 또는 “IEC 60204-1”를 참조하십시오.

*   **정지0**

    모든 조인트 모듈의 모터 전원을 즉시 제거하고 정지(제어되지 않은 정지)
*   **정지1**

    모든 조인트 모듈의 모터가 감속 후 정지하고 이후에 모터의 전원을 제거(제어 정지). 로봇은 프로그램 경로를 계속 따라가며 감속 정지하고 로봇이 정지하자마자 전원 차단
*   **정지2**

    모든 조인트 모듈의 모터가 감속 후 안전 정지 감시(SOS, Safe Operating Stop) 동작. 모든 모터의 전원 공급 유지 상태



### <mark style="color:green;">복구 모드</mark>&#xD;

안전 기능 위반으로 로봇이 정지했을 경우, 복구 모드를 통해 에러를 해제시켜 로봇을 안전한 영역으로 이동합니다. 단, 안전 보드가 FAULT 상태일 경우에는 복구 모드로 에러를 해제시킬 수 없고 재부팅해야 합니다.

### <mark style="color:green;">직접 교시</mark>&#xD;

로봇을 직접 움직여 교시하는 방법으로 로봇에 부착된 스위치로 기능을 실행합니다.