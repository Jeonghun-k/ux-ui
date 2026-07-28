# 🎨 UX/UI Study Log

> 코드는 쓸 줄 알지만 "왜 이렇게 배치했는지" 설명하지 못하던 개발자가,
> 디자인 의사결정을 언어로 설명할 수 있게 되기까지의 기록.

소프트웨어학과 재학 중인 프론트엔드 지망생의 UX/UI 학습 레포지토리입니다.
매일 하나의 개념을 배우고, **반드시 코드로 구현한 뒤, 무엇이 왜 좋아졌는지 글로 남깁니다.**

---

## 이 레포를 만든 이유

HTML/CSS/JS는 다룰 줄 알았지만, 만든 화면이 늘 어딘가 어설펐습니다.
문제는 문법이 아니라 **판단 기준의 부재**였습니다.

- 왜 이 여백은 16px인가? → "그냥 그래 보여서"
- 왜 이 글자는 굵은가? → "중요하니까"

이 레포는 그 "그냥"을 하나씩 근거 있는 규칙으로 바꿔가는 과정입니다.
디자이너가 되려는 게 아니라, **디자이너와 같은 언어로 대화하는 개발자**가 목표입니다.

---

## 학습 원칙

| 원칙 | 설명 |
|---|---|
| **매일 하나만** | 하루에 개념 1개. 넓게 훑기보다 좁게 체득 |
| **읽고 끝내지 않기** | 모든 학습은 10~20분 내 구현 과제로 마무리 |
| **회고를 남긴다** | 배운 점 / 막힌 점 / 자신감을 매일 기록 |
| **막히면 진도 안 뺀다** | 이해가 부족하면 같은 주제를 다른 예시로 반복 |

---

## 로드맵

```
1단계  디자인 기초 이론      ██████████░░░░░░  진행 중
2단계  Figma                 ░░░░░░░░░░░░░░░░  예정
3단계  HTML/CSS 퍼블리싱     ░░░░░░░░░░░░░░░░  예정
4단계  React + Tailwind      ░░░░░░░░░░░░░░░░  예정
```

<details>
<summary><b>1단계 · 디자인 기초 이론</b> — 판단 기준 만들기</summary>

- [x] UI 4대 원칙 (대비 / 반복 / 정렬 / 근접성)
- [x] 실제 서비스 UI 분석 실습
- [x] 타이포그래피 기초 (타입 스케일, 위계, 줄간격)
- [ ] 간격과 근접성 (Spacing System)
- [ ] 컬러 기초 (색상 이론, 접근성 대비비율)
- [ ] Nielsen Norman Group 10대 사용성 휴리스틱
- [ ] Laws of UX 완독

</details>

<details>
<summary><b>2단계 · Figma</b> — 손으로 그려보기</summary>

- [ ] 기본 조작 / 프레임
- [ ] 오토 레이아웃
- [ ] 컴포넌트 & Variants
- [ ] 시안 1개 직접 제작

</details>

<details>
<summary><b>3단계 · HTML/CSS 퍼블리싱</b> — 시안을 코드로</summary>

- [ ] Flexbox Froggy 완료
- [ ] Grid Garden 완료
- [ ] Figma 시안 → HTML/CSS 퍼블리싱
- [ ] 반응형 레이아웃
- [ ] 가벼운 JS 인터랙션

</details>

<details>
<summary><b>4단계 · React + Tailwind</b> — 포트폴리오</summary>

- [ ] 정적 페이지 → 컴포넌트 단위 분리
- [ ] Tailwind CSS 적용
- [ ] 포트폴리오 프로젝트 1 (기획 → 디자인 → 구현)
- [ ] 포트폴리오 프로젝트 2 (기획 → 디자인 → 구현)

</details>

---

## 학습 기록

| Day | 주제 | 실습 결과물 | 핵심 인사이트 |
|:---:|---|---|---|
| [01](./day01) | UI 4대 원칙 (CRAP) | Before/After 카드 비교 | 어수선한 디자인의 원인 대부분은 **정렬 불일치와 위계 부족**이다 |
| [02](./day02) | 실제 UI 분석 | 유튜브 홈화면 CRAP 분석 | 잘 만든 UI일수록 원칙이 안 보인다 — 안 보이는 게 정상이다 |
| [03](./day03) | `max-width` / 캡션 | 이미지 + 캡션 레이아웃 | `max-width`는 정렬이 아니라 **최대 폭 제한**. `margin: auto`가 그 여백을 나눠야 가운데 정렬이 된다 |
| [04](./day04) | 타이포그래피 위계 | 상품 카드 컴포넌트 | 강조는 크기보다 **굵기와 색**으로. 큰 글자일수록 `line-height`는 줄인다 |
| [05](./day05) | 휴리스틱 | 매일 쓰는 휴리스틱 찾기 | 사용자가 **쓰기 편하게 만드는 법**을 뜻한다|

> 각 폴더의 `README.md`에 그날의 개념 정리와 회고가 있습니다.

---

## 폴더 구조

```
.
├── README.md
├── day01/
│   ├── README.md      # 개념 정리 + 회고
│   ├── index.html
│   └── index.css
├── day02/
├── day03/
└── day04/
```

각 `dayNN/`은 **독립 실행 가능한** 정적 페이지입니다.
빌드 도구 없이 `index.html`을 브라우저로 열면 바로 확인됩니다.

---

## 기록에 남은 실제 시행착오

학습 로그에는 잘한 것만 적지 않습니다. 틀린 지점을 남겨야 다시 안 틀립니다.

**Day 2 — 근접성을 놓쳤다**
유튜브 카드에서 반복과 대비는 짚었지만, 제목·채널명·조회수가 **하나의 정보 블록으로 묶여 보이는 이유**를 설명하지 못했습니다. 간격이 그룹을 만든다는 걸 몰랐습니다.

**Day 3 — max-width를 정렬 속성으로 오해했다**
`max-width`가 가운데 정렬을 한다고 착각했습니다. 실제로는 폭을 제한할 뿐이고, 남은 여백을 `margin: auto`가 양쪽으로 나눠야 정렬이 일어납니다.

**Day 4 — 태그 선택자로 스타일을 덮어쓰고 있었다**
`span { font-size: 14px }`로 전역에 걸어놓고, 배지만 `.label`로 다시 12px로 되돌리는 구조였습니다. **주고 나서 취소하는 CSS**는 관리가 안 됩니다. 역할 기반 클래스(`.badge`, `.price`)로 리팩터링했습니다.

---

## 참고 자료

**디자인 원칙**
- [Laws of UX](https://lawsofux.com/) — UX 법칙 모음
- [10 Usability Heuristics — NN/g](https://www.nngroup.com/articles/ten-usability-heuristics-for-user-interface-design/)
- [Refactoring UI](https://refactoringui.com/) — 개발자를 위한 디자인

**타이포그래피**
- [Legibility, Readability, and Comprehension — NN/g](https://www.nngroup.com/articles/legibility-readability-comprehension/)
- [Typography Terms: Glossary — NN/g](https://www.nngroup.com/articles/typography-terms-ux/)
- [Type Scale](https://typescale.com/) — 타입 스케일 생성기

**CSS 레이아웃**
- [Flexbox Froggy](https://flexboxfroggy.com/#ko)
- [Grid Garden](https://cssgridgarden.com/#ko)
- [MDN CSS](https://developer.mozilla.org/ko/docs/Web/CSS)

**Figma**
- [Figma 공식 튜토리얼 (한국어)](https://www.figma.com/ko-kr/community/design-tutorials/figma/)

---

<div align="center">

**진행 중** · 매일 업데이트

</div>
