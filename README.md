#### 📦 Fully Autonomous Convenience Store Stocking Robot
본 프로젝트는 **인간의 개입 없이 편의점 진열·보충 작업을 수행하는 완전 무인 로봇 시스템**을 개발하는 것을 목표로 한다.
상품 인식부터 이동, 진열, 재고 갱신까지 전 과정을 자동화하는 **End-to-End 무인 진열 시스템**을 설계한다.

#### 🎯 Project Objective
- 인력 개입 없는 **완전 무인 진열 시스템 구현**
- 다양한 상품을 인식하고 분류하여 적절한 선반에 배치
- 이동형 로봇 + 로봇 팔 통합 제어
- 실제 편의점 환경을 가정한 자율 판단 로직 설계
> 본 프로젝트는 상용화를 목적으로 하지 않으며, 연구·개발 목적의 프로토타입이다.

#### 🧠System Architecture
1. Perception
   - RGB / Depth 카메라 기반 상품 인식
   - 바코드, 패키지 특징 기반 분류
   - 선반 및 빈 공간 인식
  
2. Decision & Planning
   - 상품별 진열 규칙 데이터베이스
   - 현재 진열 상태 분석
   - 작업 순서 자동 계획 (Task Planning)

3. Mobility
   - SLAM 기반 매장 자율 주행
   - 장애물 회피 및 경로 재계획

4. Manipulation
   - 로봇 팔 기반 픽앤플레이스
   - 선반 높이.각도 대응
   - 물체 안정성 고려한 그리퍼 제어

5. System Integration
   - ROS2 기반 분산 노드 구조
   - 센서-판단-제어 파이프라인 통합

___
#### 🛠 Tech Stack
- Framework
  - ROS2 (Humble)
- Languages
  - Python / C++
- Vision & AI
  - OpenCV
  - (Optional) YOLO-based Object Detection
- Navigation
  - SLAM
  - Navigation2
- Hardware (Target)
  - 이동형 로봇 플랫폼
  - 6-DOF 로봇 팔
  - RGB-D Camera
  - Adaptive Gripper
 
___
#### 🧪 Development Scope
##### Phase 1
- 정형 환경에서 무인 진열 시나리오 구현
- 제한된 상품 종류 및 고정 진열 규칙

##### Phase 2
- 다종 상품 분류
- 동적 장애물 대응
- 재고 상태 인식

##### Phase 3
- 실제 편의점 환경에 가까운 테스트
- 예외 상황 처리 로직 강화
___
#### ⚠️ Known Challenges
- 상품 포장 반사/가림 문제
- 비정형 진열 환경
- 사람 출입에 따른 동적 변화
- 물체 파지 안정성
___
#### 📌 Motivation
편의점 진열 업무는 **자동화 난이도가 높지만 반복 빈도가 매우 높은 작업**이다.
본 프로젝트는 완전 무인 환경에서 로봇이 인지-판단-행동의 전 과정을 수행할 수 있는지를 실험하는 것을 목표로 한다.

