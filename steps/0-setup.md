# 0단계. 세팅 (10분)

## 목표

스킬, 모델, AGENTS를 확인한 작업 폴더가 남는다.

## Codex에게

아래 "내가 할 것" 4번까지 끝낸 뒤 실행한다.

```
$setup-matt-pocock-skills
Issue tracker는 Local markdown, 위치는 docs/<feature>/, Domain docs는 single-context로 해줘. 다시 묻지 말고 초안 확인 없이 바로 작성해.
```

## 내가 할 것

`kit/README.md`의 설치 명령을 먼저 실행해 Codex까지 켠 상태에서 시작한다.

1. 과제 README를 정독하고 필수 제출물의 파일명과 경로, 실행 방식, 포트, 화면 요구를 적어 둔다.
2. `git status`로 저장소인지 확인한다. 아니면 `git init` 후 첫 커밋을 한다.
3. `/skills`로 14개를 확인한다. 안 보이면 Codex를 다시 켠다.
4. `/model`에서 effort를 medium으로 바꾸고 `/status`로 확인한다. 기본값이 low일 수 있다. 모든 단계를 medium으로 한다. 세션 중간에는 effort를 바꾸지 않고, 바꿔야 하면 새 세션을 시작할 때 바꾼다.
5. 위 setup을 실행한다.
6. 스킬과 키트를 별도 커밋으로 남긴다.

setup이 실패하면 AGENTS.md에 직접 쓴다:

```markdown
## Agent skills
### Issue tracker
Local markdown, GitHub 사용 안 함. 스펙은 docs/<feature>/spec.md, 티켓은 docs/<feature>/issues/NN-<slug>.md (Blocked by: 줄로 의존 표시).
### Domain docs
Single-context: 루트 GLOSSARY.md + docs/adr/.
```

Codex 업데이트 제안은 진행하지 않는다. 사용할 수 없는 포트나 경로는 공식 안내를 따른다. 터미널의 링크를 누르지 말고 플랫폼의 미리보기를 쓴다.

## 완료 조건

- [ ] 스킬 14개 확인
- [ ] 모델과 effort 확인
- [ ] AGENTS 확인
- [ ] 별도 커밋

## 시간 초과

시간이 밀리면 effort를 내리기 전에 티켓과 질문부터 줄인다. medium이 많이 느리면 사실 수집, 문서 정리, 단순 수정만 low로 하고, 판단, 명세, 핵심 구현은 medium을 유지한다. API 오류가 반복되면 effort 문제가 아니므로 문제 신고를 한다.
