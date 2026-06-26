# MSH153 AI 도구 학습 미션

이 저장소는 AI 도구 학습 과정에서 수행한 두 개의 미션 결과물을 정리한 프로젝트입니다.

- 미션 1: LLM 모델 비교와 프롬프트 설계를 통한 Q&A IBS 성경 묵상 튜터 제작
- 미션 2: AI 이미지, 영상, 오디오 도구를 활용한 Q&A IBS 브랜드 광고 영상 제작

두 미션은 모두 `Q&A IBS 성경 묵상`을 중심 주제로 삼고 있습니다. 미션 1은 텍스트 기반 LLM 활용과 프롬프트 엔지니어링에 집중하고, 미션 2는 동일한 메시지를 멀티모달 광고 콘텐츠로 확장합니다.

## 프로젝트 구조

```text
.
├── mission1/
│   ├── README.md
│   ├── mission.md
│   ├── low-lev/
│   │   ├── GPT0.md
│   │   ├── gem0.md
│   │   └── cla0.md
│   ├── v1v2-lev/
│   │   ├── claude3.md
│   │   └── claude5.md
│   └── goal-lev/
│       ├── model_comparison_report.md
│       ├── system_design.md
│       ├── log.md
│       └── prom0.md
└── mission2/
    ├── README.md
    ├── story_board.txt
    ├── story_board.pdf
    └── video.mp4
```

## 미션 1: Q&A IBS 성경 묵상 LLM 설계

미션 1은 LLM을 단순 질의응답 도구가 아니라, 초신자가 성경 본문을 관찰하고 해석하며 적용할 수 있도록 돕는 `Q&A IBS 성경 묵상 튜터`로 설계하는 과제입니다.

주요 내용은 다음과 같습니다.

- `GPT0`, `gem0`, `cla0` 세 가지 대화 결과를 비교
- 비용, 시간 사용, IBS식 묵상 적합성, 신학적 근거를 기준으로 평가
- 최종 모델로 `cla0` 선정
- 초신자를 위한 페르소나, 입력 템플릿, 시스템 프롬프트 설계
- Few-shot 예시, 단계적 추론 유도, 환각 검증 기준 구성
- 골로새서 1:1-8 본문을 기준으로 10턴 이상의 실제 묵상 로그 작성

핵심 산출물:

- [미션 안내](./mission1/mission.md)
- [모델 비교 및 선정 보고서](./mission1/goal-lev/model_comparison_report.md)
- [시스템 설계 문서](./mission1/goal-lev/system_design.md)
- [실행 로그](./mission1/goal-lev/log.md)
- [미션 1 README](./mission1/README.md)

## 미션 2: AI 기반 브랜드 광고 영상 제작

미션 2는 Q&A IBS 성경 묵상의 유익을 알리는 브랜드 광고를 기획하고, 생성형 AI 도구를 활용해 이미지, 영상, 오디오가 결합된 광고 영상으로 완성한 과제입니다.

브랜드 및 캠페인 방향은 다음과 같습니다.

- 브랜드 아이덴티티: `A Light In The Darkness`
- 핵심 메시지: `Q&A IBS! 빛되신 주님과 만나요`
- 영상 구성: 4개 씬의 애니메이션 광고
- 주제: 어려운 성경을 Q&A IBS 방식으로 묵상할 때, 오늘 말씀하시는 하나님을 만날 수 있다는 메시지

사용 도구:

- 2D 이미지 생성: Gemini
- 영상 제작: Gemini Flash
- 영상 편집: Canva
- 배경 음악: Suno
- 한국어 내레이션: 네이버 클로버 더빙

핵심 산출물:

- [스토리보드 텍스트](./mission2/story_board.txt)
- [스토리보드 PDF](./mission2/story_board.pdf)
- [완성 영상](./mission2/video.mp4)
- [미션 2 README](./mission2/README.md)

## 읽는 순서

1. [mission1/mission.md](./mission1/mission.md)에서 LLM 프롬프트 설계 과제 요구사항을 확인합니다.
2. [mission1/goal-lev/model_comparison_report.md](./mission1/goal-lev/model_comparison_report.md)에서 모델 비교 결과와 최종 선정 근거를 확인합니다.
3. [mission1/goal-lev/system_design.md](./mission1/goal-lev/system_design.md)에서 Q&A IBS 튜터의 프롬프트 설계 방식을 확인합니다.
4. [mission1/goal-lev/log.md](./mission1/goal-lev/log.md)에서 실제 묵상 대화 흐름을 확인합니다.
5. [mission2/story_board.txt](./mission2/story_board.txt) 또는 [mission2/story_board.pdf](./mission2/story_board.pdf)에서 광고 기획과 씬 구성을 확인합니다.
6. [mission2/video.mp4](./mission2/video.mp4)에서 최종 광고 영상을 확인합니다.

## 프로젝트 요약

이 프로젝트는 하나의 주제인 `Q&A IBS 성경 묵상`을 두 가지 방식으로 확장합니다.

미션 1에서는 LLM 모델 비교, 프롬프트 설계, 환각 검증, 대화 로그를 통해 텍스트 기반 AI 튜터를 설계했습니다. 미션 2에서는 그 메시지를 브랜드 광고로 재구성하고, 이미지 생성, 영상 생성, 오디오 생성, 편집 과정을 거쳐 멀티모달 콘텐츠로 완성했습니다.

따라서 이 저장소는 AI 도구를 활용해 `텍스트 설계 -> 대화형 튜터 -> 스토리보드 -> 광고 영상`으로 이어지는 전체 제작 흐름을 보여주는 학습 기록입니다.
