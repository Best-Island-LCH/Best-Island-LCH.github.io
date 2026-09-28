---
# the default layout is 'page'
icon: fas fa-diagram-project
order: 1
title: Projects
---

AI 파이프라인과 데이터 시스템을 **설계·구현·검증**까지 끝까지 만든 프로젝트들입니다.
공통 원칙은 하나입니다. **AI 출력을 그대로 믿지 않고, 코드와 검증 체계로 신뢰를 확보한다.**

---

## 🏆 포미닛 — 추억의 옷을 MCM 3D 굿즈로 재창조하는 AI

> 멋쟁이사자처럼 대학 14기 중앙해커톤 **특별상** · 2026.08 · 4인 팀

옷 사진과 사연을 입력하면 MCM 헤리티지와 융합한 디자인 3안을 제안하고, 선택한 1안을 3D 굿즈(GLB)·디지털 보증서·제품 큐레이션으로 만드는 5단계 생성 파이프라인.

- **역할**: AI 파트 — 디자인 생성, 이미지 검증 게이트, 3D 변환, FastAPI 서버, 브랜드 DB
- **핵심**: Structured Outputs와 enum 주입으로 환각을 구조적으로 차단 · AI가 만든 이미지를 다른 AI가 검수하는 게이트 · 계약 우선 개발로 무충돌 병합
- **스택**: Python, FastAPI, Pydantic, Claude Sonnet 5 / Haiku 4.5, Gemini 이미지 모델, Meshy

[📄 상세 글](/posts/fourminute-mcm-upcycled-memory/){: .btn .btn-outline-primary .btn-sm } [💻 GitHub](https://github.com/LikeLion-14th-SKHU/LikeLion-14th-TEAM04-AI){: .btn .btn-outline-secondary .btn-sm }

---

## ✈️ 항공권 가격 예측 AI — "지금 살까, 기다릴까"

> 중소벤처기업부 2026 모두의창업 **2라운드 진출** · 2026.07 ~ 진행 중 · 3인 팀

공개 데이터가 없어 매일 직접 수집하기로 한 프로젝트. 10주간 약 687만 건을 자동 수집하고, 미래 가격을 정답으로 삼는 자기지도 학습으로 "지금 사세요 / 기다리세요"를 예측합니다.

- **역할**: 팀장 — 수집 파이프라인, LightGBM 모델, 전향적 검증 체계 설계·구현
- **핵심**: PC 3대 분산 수집과 IP 차단 대응 · 기준선을 실제로 이겨야만 채택하는 규칙 · 예측을 먼저 기록하고 7일 뒤 채점하는 전향적 검증(누적 57.7만 건)에서 적중률 68.7% vs 63.0%, 건당 절약 +74%
- **스택**: Python, LightGBM, SQLite, Google Flights, SerpApi, AWS EC2

[📄 상세 글](/posts/flight-price-prediction-ai/){: .btn .btn-outline-primary .btn-sm } <span class="text-muted small">코드는 비공개 (창업 진행 중)</span>

---

## 🎓 AI 강의 분석 리포트 생성기

> 멋쟁이사자처럼 NLP 엔지니어 과정 인턴 · 2026.03 · 4인 팀

STT 강의 스크립트 15일치를 5개 카테고리·18개 항목 체크리스트로 자동 평가하고 강사용 개선 리포트를 생성.

- **역할**: STT 전처리, 평가 프롬프트 설계, 리포트 생성 LLM 파이프라인, 중간·최종 발표
- **핵심**: LLM 역할을 "분석"에서 "리포트 합성"으로 분리해 점수 불일치와 환각 제거 · 일간 결과와 15회차 누적 추세를 결합한 "고질적 약점" 경고
- **스택**: Python, Gemini 2.5 Flash-Lite, multilingual-e5

[📄 상세 글](/posts/lecture-quality-report-generator/){: .btn .btn-outline-primary .btn-sm } [💻 GitHub](https://github.com/like-lion-intern/intern-project){: .btn .btn-outline-secondary .btn-sm }

---

## 🏙️ 어디가게? — 서울 소상공인 지역·업종 분석

> 멋쟁이사자처럼 대학 13기 중앙해커톤 · 2025.08 · 3인 팀

행정동 단위 인구·업종·입지 데이터를 분석해 리포트를 제공하고, 업종을 선택하면 GPT-4o-mini로 업종 특성을 서술하고 상위 지역을 추천하는 서비스.

- **역할**: AI 파트 1인 — 데이터 처리·분석 로직, LLM 연동
- **스택**: Python, GPT-4o-mini

[📄 상세 글](/posts/첫-해커톤/){: .btn .btn-outline-primary .btn-sm }
