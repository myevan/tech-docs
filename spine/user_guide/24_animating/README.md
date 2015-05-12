애니메이팅 (Animating)
======================
<http://ko.esotericsoftware.com/spine-animating>

* 도프시트: 애니 키 시각화와 타이밍 조정 (테크닉 습득 전 숙련 필요)
* 추천 서적: 애니메이터 생존 킷 <http://www.amazon.com/The-Animators-Survival-Richard-Williams/dp/0571202284>
* 추천 문서: 애니메이션 12가지 기본 원리 <http://en.wikipedia.org/wiki/12_basic_principles_of_animation>


워크 플로우 (Workflow)
----------------------
* 대표적인 애니 작업 방법 
	* Straight ahead
	* Pose-to-Pose
	* Layered
	* Combined
* 작업 애니에 따라 적합한 조합 필요

#### 스트레이트 어헤드 (Straight ahead)

처음부터 끝까지 일일이 포즈 잡음 (가장 이해하기 쉬우면서 직관적임)

* 장점: 자연스러움
* 단점: 작업 목적 망각 가능 

→ 매우 창의적인 접근 방법 (포즈를 잡기 보다는 이동 애니에 추천)

#### 포즈-투-포즈 (Pose-to-Pose)

* 통칭 블럭킹(blocking) 
* 신규 애니 작업 시작시 선호
* 타이밍 고려 없이 주요 포즈만 빠르게 작업 후 타이밍 및 중간 움직임 채움
* 장점: 
	* 최소한의 작업으로 전반적인 움직임 완성 
	* 애니 변경 비용 저렴
* 단점: 
	* 애니 흐름 방해
	* 튀는 현상 발생
	* 부자연스러움

→ 주로 애니 작업 기획 및 다른 워크 플로우 조합

#### 스파인 포즈-투-포즈 적용

* 신규 애니 작업
	1. 주요 포즈 프레임 단위 준비
	2. 주요 포즈 프레임 타이밍 조절
	3. 보간 및 개선 작업 진행
* 기존 애니 중요 키 포즈 확인: Playback 뷰 Stepped 활성화 (모든 키 트윈 기능 비활성화됨) <http://ko.esotericsoftware.com/spine-playback> 

#### 레이어드 (Layered)

* 프레임 당 일부 부분만 작업 (나머지 부분은 감춤) 
* 모든 파트 애니가 완료될 때까지 반복
	* 예1) 모든 부분을 감추고 몸체와 팔-다리만 움직임
	* 예2) 팔 다리 감추고 몸체와 엉덩이만 움직인 후 나중에 팔-다리 애니
* 장점: 
	* 애니 집중도 상승
	* 신체 일부 움직임 애니에 적합 
* 단점: 
	* 신체에 대한 깊은 이해도 필요
	* 초기 변경시 포즈 유연성 부족
	* 파츠간 움직임 단절


#### 조합 (Combined)

* 진행 순서
	1. Pose-to-Pose: 움직임을 위한 주요 포즈 구성
	2. Straight-ahead: 애니 전반 손질
	3. Layered: 프레임 별 파트 일부 개선
* 작업 계획과 창의성의 균형 필요

#### 2차 모션 (Secondary Motion)

* 통칭 반작용(counteraction) 기본 모션에 대한 리액션
* 기본 모션 효과 증폭 및 자연스러움 증가
* 대개 기본 모션보다 약간 지연되거나 반대 방향으로 움직임 (머리 카락, 칼집, 망토 등 기본 이동과 반동)
* 일반적으로  최종 마무리 작업 시점에 진행 (미리 작업시 주요 포즈 변경 어려움)
* Straight Ahead 방식이 적합함

#### 커브 (Curves)

* 애니메이션 키 사이 전환 속도 조정
* 모든 애니에 정속 사용시 부자연스러움
* 상세 설명: 그래프 페이지 참고 <http://ko.esotericsoftware.com/spine-graph>