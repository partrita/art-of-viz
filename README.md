# ggplot2를 활용한 데이터 시각화의 기술 (The Art of Visualization with `ggplot2`)

이 저장소는 TidyTuesday 데이터 시각화를 다루는 책인 *ggplot2를 활용한 데이터 시각화의 기술*(일명 *The TidyTuesday Cookbook*)의 소스 코드를 담고 있습니다. 원본 온라인 버전은 [nrennie.rbind.io/art-of-viz](https://nrennie.rbind.io/art-of-viz/)에서 확인할 수 있습니다.

이 책은 다양한 데이터 시각화 사례 연구를 통해 데이터 탐색, 시각화 유형 선택, 디자인 구상, 그리고 R과 `ggplot2`를 이용한 구현 과정을 상세하게 다룹니다.

## 주요 내용

이 책은 네 가지 주요 섹션으로 구성되어 있습니다:

1.  **일반적인 차트도 지루할 필요는 없습니다!**: 선형 차트, 막대형 차트 등 고전적인 차트를 흥미롭게 만드는 방법.
2.  **아이콘, 글꼴 및 텍스트 활용**: 외부 글꼴 로드, 아이콘 활용, 색상 텍스트 사용법.
3.  **이미지 작업**: R에서 이미지 처리(`magick`, `imager`) 및 플롯에 이미지 통합하기.
4.  **공간 데이터 시각화**: `maps`, `sf` 등을 이용한 지도 시각화 및 공간 데이터 처리.

## 시작하기

이 프로젝트는 의존성 관리를 위해 [Pixi](https://pixi.sh/)를 사용합니다. 기존의 `renv` 대신 `pixi`를 통해 R 패키지와 시스템 의존성을 관리합니다.

### 사전 요구 사항

*   [Pixi](https://pixi.sh/)가 설치되어 있어야 합니다.

### 설치

상태를 최신으로 유지하고 의존성을 설치하려면 다음 명령어를 실행하세요:

```bash
pixi install
pixi run install-r-pkgs # conda-forge에 없는 패키지들
```

### 책 빌드하기 (렌더링)
책을 HTML 또는 PDF로 빌드하려면 다음 명령어를 사용하세요:

```bash
pixi run render
```

또는 `quarto` 명령어를 직접 사용할 수도 있습니다.

```bash
quarto render
```

## 프로젝트 구조

*   `*.qmd`: 책의 각 장을 구성하는 Quarto Markdown 파일들입니다.
*   `pixi.toml`: 프로젝트 의존성 및 태스크 정의 파일입니다.
*   `_quarto.yml`: Quarto 프로젝트 설정 및 목차 구성 파일입니다.
*   `data/`: 예제에 사용되는 데이터 파일들이 위치합니다.
*   `images/`: 책에 사용되는 이미지 및 플롯 결과물입니다.
*   `R/`: 보조 R 스크립트 함수들이 포함되어 있습니다.

## 번역

현재 이 저장소의 문서는 한국어로 번역되고 있습니다.

*   `index.qmd`: 서문
*   `introduction.qmd`: 소개
*   `author.qmd`: 저자 소개
*   각 부(Part)의 소개 페이지들

## 저작권 및 라이선스

이 책의 원저작자는 [Nicola Rennie](https://nrennie.rbind.io/)입니다. TidyTuesday 프로젝트의 데이터를 활용하여 작성되었습니다.
