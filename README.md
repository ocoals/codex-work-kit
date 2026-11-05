# Codex 작업 키트

처음 보는 실무 과제를 Codex로 풀 때 쓰는 개인 작업 지침입니다. `AGENTS.md`, 단계별 안내, 빈 기록 양식, 공개 스킬 14개만 있습니다.

- 시험 문제, 데이터, 답안 코드, 구현 코드는 없습니다.
- 공식 안내와 과제 README가 이 키트보다 항상 우선합니다.

작업 폴더 루트에서 실행합니다.

```bash
git clone --depth 1 https://github.com/ocoals/codex-work-kit kit
rm -rf kit/.git
cat kit/AGENTS.md >> AGENTS.md
mkdir -p .agents/skills
cp -R kit/skills/. .agents/skills/
codex
```

터미널의 Codex에서 줄바꿈은 `Option + Enter`, 전송은 `Enter`입니다. 메신저의 줄바꿈은 `Shift + Enter`입니다.

그다음 [steps/0-setup.md](steps/0-setup.md)부터 순서대로 따릅니다. 예외 상황에는 [steps/exceptions.md](steps/exceptions.md)의 프롬프트를 씁니다.

| 단계 | 시각(T+분) | 끝나는 조건 |
|---|---|---|
| [0 세팅](steps/0-setup.md) | 0~10 | 스킬, 모델, AGENTS 확인 |
| [1 사실 수집](steps/1-facts.md) | 10~35, 2와 동시 | 수치가 있는 패턴 3개 이상, 담당자 첫 답 |
| [2 도메인 스토리](steps/2-story.md) | 10~35, 1과 동시 | 불편함, 해결 범위, 기본 사례, 담당자 확인 |
| [3 결정 표](steps/3-decisions.md) | 35~50 | 미정 0개, 방법 수준을 사람이 결정 |
| [4 합의](steps/4-agreement.md) | 50~60 | 숫자와 확인 방법까지 담당자 답 |
| [5 명세·티켓](steps/5-spec.md) | 60~75 | 숫자 시나리오, 티켓 3~4장, handoff |
| [6 구현](steps/6-implement.md) | 75~150 | 필수 티켓, 티켓당 세션 하나 |
| [7 검증·제출](steps/7-verify.md) | 150~170 | 시나리오 결과, 한계, 제출 |

`skills/eli5`를 뺀 13개는 [mattpocock/skills](https://github.com/mattpocock/skills) 커밋 `4ae2317ddb22b046e26455e4f9c9b3aaaf62212d`에서 수정 없이 복사한 것입니다. 라이선스는 MIT이며 원문은 [licenses/mattpocock-skills-LICENSE](licenses/mattpocock-skills-LICENSE)에 있습니다. `skills/eli5`는 터미널 전용으로 수정한 것이며, 출처는 [licenses/eli5-NOTICE.md](licenses/eli5-NOTICE.md)에 있습니다.
