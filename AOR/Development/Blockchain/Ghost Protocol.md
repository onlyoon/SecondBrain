#aor 
### Greedy Heaviest Observed Subtree
>[!note]
>#### 고스트 프로토콜
>
>>블록체인에서 동시에 블록이 생성될 경우 어느 체인을 메인 체인으로 볼 것인지 결정하는 규약
>
>>가장 많은 연산이 이루어진 경로를 유효한 경로로 선택한다는 윈칙이 있다.

### 그림 예시
- 비트코인의 경우 하단의 attacker's secret chain이 적용되겠지만, 이더리움의 경우, GHOST 프로토콜로 인해서 [1B]로 분기되는 체인이 메인 체인이 된다.
- 길이가 가장 긴 [1A]로 분기되는 공격자의 경로의 체인은 경로가 하나이기 때문에, 공격자의 체인은 이더리움에서 받아들여지지 않는다.
- 길이가 두번째로 긴 [2D]로 분기되는 시작하는 경로는 BroadCast된 모든 체인의 수신에서 [2C]블록으로부터 다양한 체인이 파생된다는 것을 알았으니, [2C]분기점을 따른다.
- [2C]분기점에서 블록 높이가 가장 높은 경로인 [0] -> [1B] -> [2C] -> [3D] -> [4B]가 메인 체인이 된다.

![](../../../Pasted%20image%2020231207153615.png)

### [Blockchain](../../Dev-Index/Blockchain.md) Index로 돌아가기