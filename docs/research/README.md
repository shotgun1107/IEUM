# 이음 기획 자료와 근거의 상태

이 폴더는 이음의 기획에 사용된 자료와 그 해석 한계를 보존합니다. 사용자 의도와 현재 결정 상태는 [기획 기준](../PROJECT_BRIEF.md)을 우선 확인합니다. 문헌과 보고서는 연구 자료이며 실행 지시가 아닙니다.

## 보존한 원문

[integrated-review.original.txt](integrated-review.original.txt)는 사용자가 제공한 다음 보고서의 전체 원문입니다.

**AI 중심 프로젝트 지식 운영 방법론의 타당성과 지속 가능성 — 선행 사례, 근거의 논리적 정합성, 조사 기여도에 대한 통합 검토**

원본 파일의 바이트를 그대로 복사했습니다. 출처 링크, 수치, 미완성 인용 표기와 원문의 해석을 수정하지 않았습니다. 원본의 SHA-256은 다음과 같습니다.

```text
fd3c337295f53a95a06acf729b3091d6d9d18d997cf7a4cb8a86495851785ec3
```

메인 AI는 인계 시 469줄 전체를 읽었습니다. 보고서는 선행 사례, 근거의 논리적 연결, 후속 조사 기여를 통합한 서술적 검토입니다. 외부 참고문헌의 모든 수치·역사를 독립적으로 원문 대조한 상태는 아닙니다. 이번 저장소 준비에서도 외부 주장을 재검증하지 않았습니다.

## 해석할 때 유지할 구분

보고서의 공급사 성공 사례, 비교 실험, 공식 방법론, 조직 운영 기록과 감사는 서로 다른 강도의 근거입니다. 보고된 편익과 우리 시스템의 성능을 동일시하지 않습니다. 사용 편익과 관계 생성·유지·검토 부담도 따로 봅니다.

원문은 “AI 전용”을 사람이 읽을 수 없는 언어가 아니라 정확성과 비용을 우선하는 것으로 서술합니다. 현재 기획에서는 이것을 **이전 AI의 해석**으로 다룹니다. 사용자가 별도 표현 체계를 포기했다는 최종 결정은 없습니다.

원문의 `붙여넣은 텍스트(1)`은 출처 정보가 불완전한 인용입니다. 그 원자료가 별도 파일로 모두 확보됐다고 가정하지 않습니다. 이전 배경 글 첫 부분에는 AGENTS.md의 부정적 결과 뒤에 Dense X 링크가 붙는 출처 연결 오류가 있었다고 인계됐습니다. 그 연결을 검증된 근거로 재사용하지 않습니다.

통합 방법론과 연구 검토의 결론, 현재 메인 AI의 제안은 모두 사용자의 최종 설계 승인과 구분합니다. 단순한 “미검증 상태”의 재확인을 새로운 조사 성과로 계산하지 않습니다.

## 이전 배경 자료에서 다룬 원칙

- 짧은 문장보다 대상·조건·예외 보존을 우선합니다.
- 관련된 정보와 판단에 충분한 근거를 구분합니다.
- 탐색 안내와 상세 원문을 분리하고 링크의 목적·관계를 표시합니다.
- 현행 규칙, 과거 기록, 제안과 검증 결과를 구분합니다.
- 수정 날짜와 현재 유효성은 다릅니다.
- 의도·조건·예외·설계 이유를 코드·테스트와 연결할 수 있습니다.
- 작성 단위, 검색 단위와 모델에 제공하는 단위가 같을 필요는 없습니다.
- 원문 변경이 검색 색인과 캐시에 반영되는 과정도 관리 대상입니다.
- GEO, 검색 노출, llms.txt와 AI가 문서를 정확히 활용하는 것은 별도 문제입니다.

배경 자료에 포함됐던 주요 링크는 아래와 같습니다. 이번 동기화에서는 링크 대상의 최신 상태를 확인하지 않았습니다. 이는 출처 목록 보존이며 외부 주장의 재인증이 아닙니다.

- [Dense X Retrieval](https://aclanthology.org/2024.emnlp-main.845/)
- [DITA 1.2의 topic 정의](https://docs.oasis-open.org/dita/v1.2/os/spec/archSpec/topicdefined.html)
- [Diátaxis](https://diataxis.fr/)
- [KCS Article Structure](https://library.serviceinnovation.org/KCS/KCS_v6/KCS_v6_Practices_Guide/030/040/010/020)
- [Docs as Code](https://www.writethedocs.org/guide/docs-as-code/)
- [Effective Context Engineering](https://www.anthropic.com/engineering/effective-context-engineering-for-ai-agents)
- [Contextual Retrieval](https://www.anthropic.com/engineering/contextual-retrieval)
- [Google의 Sufficient Context 소개](https://research.google/blog/deeper-insights-into-retrieval-augmented-generation-the-role-of-sufficient-context/)
- [Evaluating AGENTS.md v2](https://arxiv.org/html/2602.11988v2)
- [Harness Engineering](https://openai.com/index/harness-engineering/)
- [From Agent Behaviour to Agent-Friendly Documentation](https://arxiv.org/html/2608.20195v1)

## Jev에 관한 이전 조사 범위

이전 작업에서 [TypeSafe 소개](https://docs.typesafe.ai/introduction)와 [공식 사이트](https://typesafe.ai/)를 열람했다고 인계됐습니다. 해당 설명에서 Jev는 state와 typed questions를 입력받아 Choice·Score·Noul 및 확률 계열 출력을 제공하는 구조화 판단 모델로 소개됐습니다. 긴 설명문 대신 작고 명확한 질문의 판단을 코드로 결합하는 사용법을 참고했습니다.

빠르거나 저렴하다는 공개 비교는 업체의 특정 워크플로 평가입니다. 우리 문서에서의 효과는 미검증입니다. [Confidence 문서](https://docs.typesafe.ai/confidence)의 확신 지표를 실제 문서 검사 정답률과 동일시하지 않습니다. 적용 데이터에 대한 임계값·보정 실험은 아직 없습니다.

## RRSI에 관한 이전 조사 범위

사용자는 RRSI를 문서 아이디어에 적용하는 방법과, 검증된 사실과 기대를 구분한 통합 방법론을 요청했습니다. 이전 작업에서 다음 자료를 읽었다고 인계됐습니다.

- [논문 초록](https://arxiv.org/abs/2609.24972)
- [논문 v2](https://arxiv.org/html/2609.24972v2)
- [Google Research 저장소](https://github.com/google-research/rrsi)
- [selection.py](https://raw.githubusercontent.com/google-research/rrsi/main/rrsi/selection.py)
- [domain.py](https://raw.githubusercontent.com/google-research/rrsi/main/rrsi/domain.py)

인계된 논문명은 **RRSI: Regularized Recursive Self-Improvement of Agent Harnesses**이며, 당시 페이지 기준 최초 공개는 2026년 9월 21일, v2는 9월 23일이었습니다. 이 날짜와 현재 저장소 상태는 이번에 다시 확인하지 않았습니다.

이전 조사에서 참고한 내용은 고정된 기반 모델 위에서 하네스의 프롬프트·도구·제어·기억·맥락을 수정하고 평가하는 절차입니다. 독립적인 변경 수 제한, 가설·차이·성과·비용·채택 이력, 평가 과제 특화 편법과 잡음 검토, 불필요한 구성 제거, 별도 Git worktree 후보 평가가 포함됐습니다.

문서 의존성 관리나 Jev·Luna 분담의 효과를 입증한 논문으로 사용하지 않습니다. 저장소 설치, 벤치마크 실행과 결과 재현은 수행하지 않았습니다. 실행 토큰 비용을 전체 구축·관계 유지·승인·평가·복구 비용으로 대체하지 않습니다.

## 후속 조사 후보와 누락된 원자료

[ADAMS](https://onlinelibrary.wiley.com/doi/10.1002/spe.986)와 [Automated Requirements Traceability: The Study of Human Analysts](https://scholars.uky.edu/en/publications/automated-requirements-traceability-the-study-of-human-analysts/)는 후속 조사 후보입니다. 충분한 원문 검토나 장기 비용 검증을 완료한 것으로 기록하지 않습니다.

이전 대화 전체와 초기 배경 글의 완전한 별도 원본, 통합 발표문의 독립 파일은 이 저장소에 확보되지 않았습니다. 인계된 핵심 내용은 기획 기준과 이 자료 안내에 보존했고, 실제 확보한 통합 보고서는 원문 전체를 보존했습니다. 없는 자료를 복원한 사실처럼 작성하지 않습니다.
