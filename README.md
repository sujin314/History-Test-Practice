# Selenium 기반 웹앱 기능 테스트 자동화 – 식단 추천 플랫폼 QA 프로젝트

## 1. 프로젝트 개요
- Selenium 기반 자동화 테스트를 적용한 식단 추천 플랫폼 QA 프로젝트입니다.
- 현재는 서버가 만료되어 실행은 불가합니다.

---

## 2. 프로젝트 구조
```bash
├── pages/              # 기능별 페이지 객체 (현재: 히스토리)
├── utils/              # 팀 공용 유틸 함수 (로그인 등)
├── tests/              # 자동화 테스트 코드 (Selenium + Pytest)
├── .gitignore          # 환경파일 및 캐시 제외
└── README.md
```

---

## 3. 설치, 실행 방법
```bash
pip install selenium pytest
pytest -v
```
⚠️ 현재 서버 환경은 종료되었으며, 테스트 실행 흐름은 코드 및 문서로 확인 가능합니다

---

## 4. 예시 테스트 코드
```bash
#첫 번째 후기의 내용 가져오기
first_review = review[0].get_attribute("innerHTML")
assert "혼밥" in first_review, "❌ 후기가 정상적으로 작성되지 않았습니다."
print("✅ 후기가 정상적으로 작성되었습니다.")
time.sleep(1)
```
