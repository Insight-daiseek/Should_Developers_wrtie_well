# 문서 유형별 체크리스트 예시

이 폴더는 문서 유형에 따라 체크리스트를 조합하는 예시다. 문서를 작성하거나 수정할 때는 공통 체크리스트 3개를 먼저 적용한 뒤, 문서 유형에 맞는 기본 체크리스트와 세부 유형 체크리스트를 각각 하나씩 적용한다.

## 선택 순서

1. 독자가 특정 정보를 찾아 읽는가? 그렇다면 `10_reference_documents/`를 선택한다.
2. 독자가 처음부터 끝까지 읽으며 논리를 따라가는가? 그렇다면 `20_reading_documents/`를 선택한다.
3. 독자, 목적, 문서 유형이 불명확하면 추정하지 말고 `확인 필요`로 보고한다.

## 조합 예시

```text
기능 매뉴얼
├─ 00_common/01_common_quality.md
├─ 00_common/02_reader_and_topic.md
├─ 00_common/03_outline.md
├─ 10_reference_documents/10_reference_base.md
└─ 10_reference_documents/12_feature_manual.md

프로젝트 README
├─ 00_common/01_common_quality.md
├─ 00_common/02_reader_and_topic.md
├─ 00_common/03_outline.md
├─ 10_reference_documents/10_reference_base.md
└─ 10_reference_documents/17_project_readme.md

개발 보고서
├─ 00_common/01_common_quality.md
├─ 00_common/02_reader_and_topic.md
├─ 00_common/03_outline.md
├─ 20_reading_documents/20_reading_base.md
└─ 20_reading_documents/21_development_report.md

기술 설계 문서
├─ 00_common/01_common_quality.md
├─ 00_common/02_reader_and_topic.md
├─ 00_common/03_outline.md
├─ 20_reading_documents/20_reading_base.md
└─ 20_reading_documents/25_technical_design_document.md

모델 개발 업무 보고서
├─ 00_common/01_common_quality.md
├─ 00_common/02_reader_and_topic.md
├─ 00_common/03_outline.md
├─ 20_reading_documents/20_reading_base.md
├─ 20_reading_documents/21_development_report.md
└─ 20_reading_documents/24_model_development_report.md
```

## 유형 목록

| 읽기 방식 | 세부 문서 유형 |
| --- | --- |
| 사전형 | 프로덕트 매뉴얼, 기능 매뉴얼, 절차서, 외부 기능 명세서, 기능 구현 명세서, 프로젝트 README |
| 읽기형 | 개발 보고서, 모델 개발 업무 보고서, 프로덕트 제안서, 기술 블로그, 기술 설계 문서 |
