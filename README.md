# Sujee Cho

**질문을 행동으로 옮기는 사람**

일하면서, 생활하면서 떠오른 질문을 그냥 넘기지 않고 AI와 함께 직접 만들어 보며 답을 찾습니다.

`발견` → `경험과 AI로 구체화` → `직접 만들기` → `검증하고 다시 고치기`

---

## 대표 프로젝트

### 1. EnergyFlex · 사회 문제에서 시작한 질문

<sub>※ 참고 저장소: [energyflex-heat-recovery](https://github.com/sujee5947-create/energyflex-heat-recovery)</sub>

> 데이터센터는 열을 버리고, 옆 건물은 연료를 태워 난방합니다. 이 열을 옮겨 쓰면 얼마나 줄일 수 있을까?

- **만든 것**: 1 MW급 AI 데이터센터와 이웃 건물 난방을 1년 8,760시간 단위로 계산하는 시뮬레이터 (수랭, 외기냉방, 히트펌프 폐열 회수)
- **결과**: 같은 AI 작업과 같은 난방을 유지하면서, 기존 공랭 방식 대비 1차에너지 약 19.5 % 절감 (서울과 비슷한 가상 기후 가정)
- **고친 것**: 냉각기 용량을 넘는 운전이 1,730시간 섞여 있던 오류를 찾아 0시간으로 수정하는 등, 검토에서 나온 오류와 수정 과정을 모두 기록
- **한계**: 냉각 모델만 공개 실측 데이터로 검증했고, 부하와 설비는 가정입니다. 한계를 [보고서](https://github.com/sujee5947-create/energyflex-heat-recovery/blob/main/docs/EnergyFlex_Report_KR.pdf) 13장에 정리했습니다.

`Python` `NumPy` `pandas` `SciPy` `matplotlib`

### 2. BOOKMATE · 일상에서 시작한 질문

<sub>※ 참고 저장소: [bookmate](https://github.com/sujee5947-create/bookmate)</sub>

> 독서 모임에서 좋은 이야기가 오가도, 끝나면 아무것도 남지 않습니다. 기록으로 남길 수 없을까?

- **만든 것**: 모임을 녹음하면 AI가 요약하고, 토론 질문과 다음 책을 제안하는 모바일 웹앱
- **결과**: 친구들과 실제 모임에서 쓰면서 계속 고치는 중
- **고친 것**: 처음 계획(내 PC에서만 동작, 빠른 음성 인식)을 "친구들이 실제로 쓸 수 있는가"를 기준으로 여러 번 바꿈

`JavaScript` `Supabase` `Python` `Google Cloud Speech-to-Text` `Claude`

### 3. 분석 자동화 도구 · 일터에서 시작한 질문

<sub>※ 참고 저장소: [measurement-validation-automation](https://github.com/sujee5947-create/measurement-validation-automation) · [battery-quality-analysis](https://github.com/sujee5947-create/battery-quality-analysis) · [electrode-manufacturing-spc](https://github.com/sujee5947-create/electrode-manufacturing-spc)</sub>

> 같은 분석을 매번 손으로 반복해야 할까?

raw 데이터만 넣으면 통계 분석과 보고서까지 나오는 도구들입니다. 결과는 수식 검토와 통계 분석으로 검증했습니다.

| 도구 | 하는 일 |
|---|---|
| [measurement-validation-automation](https://github.com/sujee5947-create/measurement-validation-automation) | 두 측정 장비의 일치도(Bland–Altman, 반복성) 판정, Excel·HTML·PPT 보고서 자동 생성 |
| [battery-quality-analysis](https://github.com/sujee5947-create/battery-quality-analysis) | 측정 데이터의 규격 판정, 공정 성능 지수(Pp/Ppk), 상관 분석 대시보드 |
| [electrode-manufacturing-spc](https://github.com/sujee5947-create/electrode-manufacturing-spc) | 제조 공정 SPC 관리도(I-MR, C, U), 공정능력(Cp/Cpk), 불량 패턴 분석 |

---

## 그 밖의 시도

- [flashcard](https://github.com/sujee5947-create/flashcard): 영어 단어·표현 암기용 플래시카드 웹앱
- [TK-travel-plan](https://github.com/sujee5947-create/TK-travel-plan): 여행 일정과 동선을 관리하는 웹앱

---

**일하는 원칙**  모르면 배운다 · 의심되면 검증한다 · 불편하면 개선한다 · 한계는 숨기지 않는다 · 가설은 데이터로 검증한다
