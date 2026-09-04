# 한의원 AI 경영컨설턴트

한의원 AI 경영컨설턴트는 스크린샷, PDF, Excel, Clipboard 데이터를 이용해 한의원의 경영 데이터를 정리·누적하고 변화 추이를 분석하는 Windows 프로그램입니다.

특정 차트 프로그램과 직접 연동하지 않습니다. 각자의 차트 환경에서 스크린샷, PDF, Excel 또는 `Ctrl+C` / `Ctrl+V`만으로 데이터를 입력할 수 있습니다.

모든 경영 데이터는 사용자의 컴퓨터에만 저장됩니다. 개발자는 매출, 환자 수, OCR 결과, PDF, Excel 등 어떠한 사용자 데이터도 수집하거나 확인하지 않습니다.

## 최신 버전 다운로드

### v1.7.1 - 2026-09-04

[![Windows EXE 다운로드](https://img.shields.io/badge/Windows_EXE-v1.7.1-0A66C2?style=for-the-badge&logo=windows)](https://github.com/themeischaos-star/hani-ai-consultant-release/releases/download/v1.7.1/hani-ai-consultant-v1.7.1.exe)

- 파일: `hani-ai-consultant-v1.7.1.exe`
- 운영체제: Windows 10/11 64-bit
- 설치: 별도 설치 없이 EXE 실행
- SHA-256: `bb5b468ad433e48ec0e44ad12cab3a7a6c41837e76ba5edb05f9891cb9948e1c`
- [Release Notes](https://github.com/themeischaos-star/hani-ai-consultant-release/releases/tag/v1.7.1)
- [상세 사용설명서](docs/USER_GUIDE.md)
- [사용설명서 PDF](https://github.com/themeischaos-star/hani-ai-consultant-release/releases/download/v1.7.1/user_guide-v1.7.1.pdf)

> 다운로드한 EXE의 SHA-256이 위 값과 일치하는지 확인해 주세요. 값이 다르면 실행하지 마세요.

## Windows 보안 경고 안내

현재 개인 개발 프로젝트로 Code Signing 인증서가 적용되지 않았습니다. 처음 실행할 때 Windows SmartScreen의 `Windows의 PC 보호` 경고가 나타날 수 있습니다.

공식 Release에서 내려받았고 SHA-256이 일치한다면 다음 순서로 실행할 수 있습니다.

1. 경고 화면에서 `추가 정보`를 선택합니다.
2. 게시자와 파일명을 다시 확인합니다.
3. `실행`을 선택합니다.

코드 서명이 적용되지 않은 새로운 개인 개발 프로그램에서 나타날 수 있는 일반적인 경고입니다. 출처가 불분명하거나 SHA-256이 다른 파일은 실행하지 마세요.

## 백신 프로그램 안내

일부 백신은 새로 배포된 실행파일을 기본적으로 검사하거나 차단할 수 있습니다. v1.7.1 배포본은 Microsoft Defender 검사에서 `위협 없음`을 확인한 뒤 배포됐습니다.

실행이 차단되면 먼저 공식 Release와 SHA-256을 확인하고, 사용하는 백신의 검사 결과를 확인하세요. 검증이 끝난 공식 파일에 한해서만 해당 백신의 예외 등록 기능을 사용할 수 있습니다.

## 개인정보 안내

- 자료와 설정은 사용자의 Local PC에 저장됩니다.
- 프로그램은 한의원 데이터를 개발자 서버로 전송하지 않습니다.
- 개발자는 매출, 환자 수, OCR 결과, PDF, Excel을 열람하거나 수집할 수 없습니다.
- OpenAI API Key를 요구하거나 저장하지 않습니다.
- `AI 분석`을 선택했을 때만 사용자가 검토한 Markdown을 Clipboard로 복사하고 ChatGPT를 엽니다.
- ChatGPT에 붙여넣기 전 환자 식별정보가 없는지 사용자가 최종 확인해야 합니다.

## 프로그램 사용 흐름

```text
자료 입력
   ↓
OCR·표 확인 및 수정
   ↓
Database 저장
   ↓
일간·월간·연간 추세 분석
   ↓
필요할 때만 ChatGPT AI 분석
```

## 지원 형식

| 구분 | 지원 형식 |
|---|---|
| 이미지 | PNG, JPG, JPEG |
| 문서 | PDF |
| 표 파일 | XLS, XLSX, CSV |
| Clipboard | 이미지, 텍스트, 숫자, 표, Excel 셀, TSV, CSV, HTML Table |

## 주요 기능

- 이미지·스캔 PDF OCR과 낮은 신뢰도 숫자 확인
- OCR 이상값 검증 및 사용자 수정값 저장
- 경영 데이터의 일간·월간·연간 누적
- 시계열 분석과 전일·전주·전월·전년 동월 비교
- KPI Dashboard와 목표 달성률
- 100점 Health Score와 산정 근거
- Timeline과 Business Journal
- 월간 경영보고서와 PDF 저장
- 경영 시뮬레이션, 3·6·12개월 예측, 개선과제
- 경영 캘린더 Heat Map과 날짜별 Business Time Machine
- 전일·동일요일·전월·전년 자동 비교와 AI 비교 브리핑
- 사용자의 ChatGPT를 이용하는 선택적 AI 분석

## 처음 사용하는 방법

1. 최신 EXE를 내려받아 실행합니다.
2. 최초 실행 안내에 따라 한의원 정보와 KPI를 입력합니다.
3. `파일 선택`, 드래그앤드롭 또는 `Ctrl+V`로 자료를 넣습니다.
4. OCR·표 결과를 확인하고 틀린 숫자를 수정합니다.
5. Database 저장 후 `데이터 분석`에서 추세를 확인합니다.
6. 원인·개선전략이 필요할 때만 `AI 분석`을 선택합니다.

자세한 설명은 [사용설명서](docs/USER_GUIDE.md)와 [FAQ](docs/FAQ.md)를 확인하세요.

## 주의사항

- OCR 결과는 저장 전에 반드시 한 번 확인해 주세요.
- OCR 오류는 검수 표에서 수정한 뒤 저장하면 Database에 반영됩니다.
- 경영 분석과 미래 예측은 참고 자료이며 최종 의사결정은 사용자가 직접 판단해야 합니다.
- AI 분석 결과도 참고용으로 활용하세요.
- 환자 이름, 연락처, 주민등록번호 등 식별정보는 업로드하거나 ChatGPT에 전달하지 마세요.

## 업데이트

새 버전은 이 저장소의 [Releases](https://github.com/themeischaos-star/hani-ai-consultant-release/releases)에서 제공합니다. 업데이트 전 기존 데이터 폴더를 백업하고, 최신 EXE를 내려받아 기존 EXE 대신 실행하세요. 사용자 데이터와 환경설정은 EXE와 분리되어 보존됩니다.

버전별 변경사항은 [CHANGELOG](CHANGELOG.md)를 확인하세요.

## 문의 전 확인

오류가 발생하면 먼저 다음 내용을 확인해 주세요.

- 사용 중인 프로그램 버전
- Windows 10/11 64-bit 여부
- 입력 파일 형식
- OCR 원본의 해상도와 글자 선명도
- [자주 발생하는 오류](docs/USER_GUIDE.md#자주-발생하는-오류)

이 저장소는 공식 다운로드와 사용 안내를 위한 Public Repository입니다. 개발 소스와 사용자 데이터는 포함하지 않습니다.
