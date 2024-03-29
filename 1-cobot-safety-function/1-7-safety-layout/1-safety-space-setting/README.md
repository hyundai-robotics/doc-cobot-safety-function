﻿# 1.7.1 안전 영역 설정

안전 영역은 툴 및 로봇 엘보우 영역을 모니터링하기 위한 작업 공간 또는 보호 공간입니다. 작업 공간은 모니터링 대상이 자유롭게 움직일 수 있지만 떠날 수는 없는 제한된 공간입니다. 이와 달리, 보호 공간은 모니터링 대상이 진입하면 움직일 수 없는 제한된 공간입니다. 안전 영역이 작업 공간일 경우 안전 조건 번호를 할당하여 이를 활성화할 수 있습니다. 작업 공간에서 안전 조건의 한계값이 초과하여 동작하면 기능별 안전 정지가 활성화됩니다.

![그림 6 안전 영역: 작업 공간](<../../../_assets/image_3.png>)

![그림 7 안전 영역: 보호 공간](<../../../_assets/image_4.png>)

안전 영역은 로봇 좌표계를 기준으로 원점의 위치와 길이를 설정하고 정지 거리를 포함하여 구성합니다. 직육면체의 공간으로 최대 12 개까지 추가할 수 있습니다. 안전 공간은 파라미터 설정 또는 안전 I/O 신호에 의해 활성화됩니다.

안전 영역을 설정하는 방법은 다음과 같습니다.

1\. **\[설정]** 버튼 > **\[4: 응용 파라미터 > 21: 협동로봇 설정 > 1: 안전 기능 > 2: 안전 레이아웃]** 메뉴를 터치하십시오.

2\. 안전 영역 유형을 선택하고 파라미터 값을 설정한 후 **\[적용]** 버튼을 터치하여 저장하십시오.

![](../../../_assets/image31.jpeg)

|                 **번호**                | 　　　　　　　　　　　**설명**                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| :-----------------------------------: | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|  ![](../../../_assets/1.png)  | 안전 영역의 상세 정보입니다. 영역의 이름과 파라미터 값을 확인 및 설정할 수 있습니다. 설정 정보에 대한 자세한 내용은 “[**1.7.1.1 안전 영역 파라미터 설정 정보**](1-1-safety-space-parameter-setting-info.md)”를 참조하십시오.                                                                                                                                                                                                                                                                                                            |
|  ![](../../../_assets/2.png)  | <ul><li><strong>[툴]</strong>: 안전 영역 모니터링에 사용하는 툴의 파라미터 값을 설정합니다. 자세한 내용은 “<a href="../2-safety-tool-modeling.md"><strong>1.7.2 안전 툴 모델링</strong></a>”을 참조하십시오.</li><li><strong>[로봇]</strong>: 안전 공간 모니터링에 사용하는 로봇 모델의 파라미터 값을 설정합니다. 자세한 내용은 “<a href="../3-safety-robot-modeling.md"><strong>1.7.3 안전 로봇 모델링</strong></a>”을 참조하십시오.</li></ul>                                                                                                                       |
|  ![](../../../_assets/3.png)  | <ul><li><strong>[적용]</strong>: 변경 내용을 저장합니다.</li><li><strong>[+]</strong>/<strong>[-]</strong>: 새로운 안전 영역을 추가하거나 안전 영역을 삭제합니다. 안전 영역은 최대 12 개까지 추가할 수 있습니다.</li><li>안전 영역 목록입니다. 영역 이름을 선택하면 상세 정보를 확인 및 수정할 수 있습니다.</li><li><p><strong>[페이지 복사]</strong>/<strong>[페이지 붙여넣기]</strong>: 안전 영역 정보를 복사하여 다른 영역에 붙여 넣습니다.
</p><p>목록에서 복사할 영역 정보의 이름을 선택하고 <strong>[페이지 복사]</strong> 버튼을 터치한 후 값을 적용할 영역의 이름을 선택하고 <strong>[페이지 붙여넣기]</strong> 버튼을 터치하십시오.
</p></li></ul> |

3\. 파라미터 값을 확인한 후 **\[X]** 버튼을 터치하거나 티치 펜던트의 **\<esc>** 키를 눌러 설정을 종료하십시오.
