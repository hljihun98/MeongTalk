# 멍톡 AI — 강아지 한국어 통역기 MVP

## 실행 방법
1. 이 폴더를 로컬 서버로 실행합니다.
   - VS Code Live Server 사용 또는
   - `python -m http.server 5173`
2. 브라우저에서 `http://localhost:5173` 접속
3. 마이크/카메라 권한 허용

## 포함 기능
- Web Audio API 기반 마이크 입력
- 자동 게인/노이즈 억제 옵션 요청
- RMS, 피치 근사, Zero Crossing Rate 기반 소리 특징 추출
- Bark / Whine / Growl / Howl / Panting / Sniff 휴리스틱 분류
- 상황 데이터와 결합한 감정/의도 점수 계산
- 한국어 통역 문장 생성
- 위험 알림: 통증 의심, 공격성, 불안
- 보호자 피드백 로컬 저장
- jsPDF 기반 PDF 리포트 저장
- PWA manifest / service worker 포함

## 실제 AI 모델로 고도화할 부분
- TFLite Audio CNN + BiLSTM/Transformer 모델 연결
- MediaPipe/YOLO 기반 강아지 keypoint 추정
- 보호자 피드백 기반 개인화 파인튜닝
- 품종/나이/건강 상태별 보정

## 주의 문구
이 앱은 수의학적 진단이 아니라 행동·음성 기반 추정 도구입니다.
