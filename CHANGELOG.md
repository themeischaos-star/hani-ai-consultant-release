# 변경 기록

## v2.0 - Medical Intelligence OS

- Dashboard 중심 6개 작업공간 UI
- 현재 확보된 KPI만 나타나는 카드와 Optional Intelligence
- 통합 자료 입력, Reports, Data Center, Settings
- 1366·1600·1920·2560 Windows UI 검증
- DB 스키마 3과 기존 OCR·분석·기록·보고서 기능 유지

# 변경사항

## v1.7.1 - 2026-09-04

### Business Time Machine

- 월 평균 대비 총매출을 색상으로 보여주는 경영 캘린더 Heat Map
- 날짜 선택 시 KPI, Dashboard 상태, Health Score, Timeline, 경영일지, 개선과제 복원
- 전일, 직전 동일요일, 최근 4주 동일요일 평균, 전월·전년 동일요일 자동 비교
- 작년 같은 주와 전년 동월을 포함한 사용자 선택형 비교 설정
- 비교 결과 한 줄 브리핑, Dashboard 자동 비교, Data Coach 부족 구간 안내
- 월간·분기·연간 비교가 포함된 월간 실행 리뷰

### 호환성과 배포

- Database 스키마 3 유지, 기존 데이터 마이그레이션 불필요
- 기존 OCR·Excel·PDF·Clipboard·Dashboard·Timeline 기능 유지
- Windows EXE smoke test 및 Microsoft Defender 검사 통과

## v1.6.1 - 2026-09-02

### 경영 분석

- OCR 음수·매출 합계 모순·이상치·급증·급감·날짜 역순 검증
- 최근 30일과 이전 30일 KPI 상태 및 자동 Insight
- 목표 달성률, KPI 알림과 100점 Health Score 근거
- Timeline 전후 변화 연결과 Business Journal
- 월간 경영보고서 Markdown·PDF

### 예측과 실행

- 신환·재진율·삼진율·객단가·예약률·보험 구성·유입경로·LTV 시뮬레이션
- 예상 월매출·연매출과 3·6·12개월 추세 예측
- 목표 매출까지 필요한 환자·객단가·예약률 격차 계산
- 우선순위 개선과제와 완료 체크
- 개선과제 완료 시 Timeline·Business Journal 자동 기록
- Dashboard 최우선 과제와 월간 실행 리뷰

### 배포 품질

- Windows 10/11 64-bit 설치 없는 EXE
- UPX 미사용 Release Build
- Version Resource와 프로그램 아이콘
- 개인정보·사용자 설정 자동 제외 및 최초 실행 상태 보장
- Windows EXE smoke test 통과
- Microsoft Defender 검사 결과 위협 없음

이 Public Repository에는 v1.6.1부터 사용자용 변경사항을 제공합니다.
