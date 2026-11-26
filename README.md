### 🔭 Projects

| | 프로젝트 | 한 줄 소개 | 기술 |
|---|---|---|---|
| 💡 | **Lumo** | 말한 물건 위에 빛을 비추고 "3시 방향"으로 안내하는 저시력자용 탐색 시스템 · 🥇 교내 금상 | YOLOE · Whisper · RealSense |
| 📱 | [**디딤**](https://apps.apple.com/kr/app/%EB%94%94%EB%94%A4-%EC%A0%80%EC%8B%9C%EB%A0%A5%EC%9E%90-%EB%AC%BC%EA%B1%B4-%EC%B0%BE%EA%B8%B0/id6829758026) | Lumo를 스마트폰으로, 화면 밖 물건까지 방향·거리로 안내하는 앱 · 앱스토어 출시 | ARKit · SLAM |
| 🎬 | **개인형 4D 기기** | 영상만 보고 진동·바람·온냉 4D 효과를 자동 생성 *(진행 중)* | Qwen3-VL · Qwen2.5-Omni |
| 🎾 | [**스쿼시 분석**](https://github.com/dlsy4501/squash_pose_coach) | 카메라 앵글 오차를 줄인 자세 비교 + 랠리 전체 분석으로 차별화한 스쿼시 코칭 앱 | YOLO11-pose · OpenCV |
| 🎲 | [**메르칸티스**](https://github.com/dlsy4501/Mercantis_boardgame) | 직접 설계한 보드게임을 실시간 멀티플레이 웹으로 · [▶ 플레이](https://mercantis.onrender.com/) | Node.js · Socket.io |
| 🧪 | [**YOLOv1-ResNet101**](https://github.com/dlsy4501/2025-computer-vision) | YOLOv1 직접 구현 및 작은 물체 탐지 개선 | PyTorch |

<details>
<summary>🎾 스쿼시 분석 — 기존 서비스와의 차별점</summary>

기존 스윙·자세 분석 앱(골프·테니스용 AI 코치 다수 포함)은 대부분 영상 속 자세를 **하나의 "이상적인" 레퍼런스 자세**와 각도만 비교합니다. 이 방식은 촬영 카메라 각도가 레퍼런스와 다르면 괜찮은 자세도 "틀렸다"고 판정하기 쉽습니다.

- **카메라 앵글 오차 보정**: 어깨너비·몸통길이 비율로 몸이 카메라를 얼마나 정면으로 보고 있는지 근사하고, 비교 시점마다 나와 방향이 비슷한 레퍼런스 샘플만 걸러서 평균±표준편차를 계산합니다. 깊이 센서나 멀티카메라 없이 스마트폰 영상 한 대로도 각도 차이로 인한 오탐을 줄이는 방식입니다.
- **스윙 한 순간이 아니라 경기 전체를 봄**: 대부분의 자세 교정 앱은 임팩트 한 프레임에만 초점을 맞추지만, 이 프로젝트는 선수 추적·이동 거리·코트맵·랠리/득점 추정까지 더해 경기 흐름 전체를 중계 화면처럼 보여주는 분석 엔진을 함께 제공합니다.
- **특수 장비 없이 동작**: 깊이 카메라나 멀티카메라 설치 없이, 고정 카메라(삼각대) 영상만으로 돌아갑니다.

</details>

---

### 🛠 Tech Stack

**Vision & AI**<br/>
<img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" />
<img src="https://img.shields.io/badge/YOLO-111F68?style=flat-square&logo=yolo&logoColor=white" />
<img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white" />
<img src="https://img.shields.io/badge/Whisper-412991?style=flat-square&logo=openai&logoColor=white" />
<img src="https://img.shields.io/badge/Qwen--VL-615CED?style=flat-square" />
<img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white" />
<img src="https://img.shields.io/badge/LightGBM-02569B?style=flat-square" />
<img src="https://img.shields.io/badge/RealSense-0071C5?style=flat-square&logo=intel&logoColor=white" />

**Mobile & Web**<br/>
<img src="https://img.shields.io/badge/ARKit-000000?style=flat-square&logo=apple&logoColor=white" />
<img src="https://img.shields.io/badge/Android-3DDC84?style=flat-square&logo=android&logoColor=white" />
<img src="https://img.shields.io/badge/Node.js-5FA04E?style=flat-square&logo=nodedotjs&logoColor=white" />
<img src="https://img.shields.io/badge/Socket.io-010101?style=flat-square&logo=socketdotio&logoColor=white" />
<img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black" />
<img src="https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white" />
<img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white" />

**Languages & Tools**<br/>
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white" />
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" />
<img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" />
<img src="https://img.shields.io/badge/Bitbucket-0052CC?style=flat-square&logo=bitbucket&logoColor=white" />

---

### 📫 Contact

<a href="https://dlsy4501.github.io/portfolio/"><img src="https://img.shields.io/badge/Portfolio-171B23?style=for-the-badge&logo=googlechrome&logoColor=white" /></a>
<a href="https://www.instagram.com/dlsy4501/"><img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white" /></a>
