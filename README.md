# 웹 서비스 성능 개선 보고서

## 1. 개요

- **평가 도구**: PageSpeed Insights
- **평가 URL**:
    - 최초:
        - [모바일 성능 평가](https://pagespeed.web.dev/analysis/https-hanghae-assignment-9-3175c-web-app/ae5z45tc9c?form_factor=mobile)
        - [데스크톱 성능 평가](https://pagespeed.web.dev/analysis/https-hanghae-assignment-9-3175c-web-app/ae5z45tc9c?form_factor=desktop)
    - 최종:
        - [모바일 성능 평가](https://pagespeed.web.dev/analysis/https-hanghae-assignment-9-3175c-web-app/2et73t8t4t?form_factor=mobile)
        - [데스크톱 성능 평가](https://pagespeed.web.dev/analysis/https-hanghae-assignment-9-3175c-web-app/2et73t8t4t?form_factor=desktop)
- **평가 일자**: 2024.08.14

## 2. 성능 평가 결과 요약

### 2-1. 수치 비교 (개선 전 → 후)

- 성능 점수
    - 모바일: **32 → 99**
    - 데스크톱: **51 → 100**
- 접근성 점수
    - 모바일: **82 → 100**
    - 데스크톱: **82 → 100**
- 검색엔진 최적화
    - 모바일: **82 → 100**
    - 데스크톱: **82 → 100**
- 주요 지표:
    - First Input Delay (FID)
        - 모바일: **2.4s → 0.8s**
        - 데스크톱: **0.6s → 0.3s**
    - Largest Contentful Paint (LCP)
        - 모바일: **11.7s → 1.9s**
        - 데스크톱: **3.1s → 0.5s**
    - Cumulative Layout Shift (CLS)
        - 모바일: **0.405 → 0**
        - 데스크톱: **0.513 → 0**

### 2-2. 개선 효과 분석

- 성능 점수가 데스크톱과 모바일 환경에서 각각 50% 이상 증가했으며, 이로 인해 사용자 경험이 개선되었습니다.
- FID가 데스크톱 환경에서는 50%, 모바일 환경에서는 약 67% 감소했으며, 이로 인해 사용자 상호작용에 대한 응답 시간이 개선되었습니다.
- LCP가 데스크톱과 모바일 환경에서 각각 약 84% 감소했으며, 이로 인해 페이지 최초 로딩 시간이 개선되었습니다.
- CLS가 데스크톱과 모바일 환경에서 모두 0으로 감소했으며, 이로 인해 레이아웃 안정성이 개선되었습니다.

## 4. 성능 개선 작업 상세

### 4.1 이미지 최적화

- 작업 내용: 모든 이미지를 WebP 형식으로 변환하고, Lazy Loading을 적용하여 초기 페이지 로딩 속도를 개선했습니다.
- 개선 효과: LCP가 모바일에서 11.7초에서 1.9초로, 데스크톱에서 3.1초에서 0.5초로 개선되었습니다.

### 4.2 자바스크립트 최적화

- 작업 내용: 불필요한 자바스크립트 파일 제거하여 자바스크립트 로딩 시간을 단축했습니다.
- 개선 효과: FID가 모바일에서 0.8초, 데스크톱에서 0.3초로 크게 개선되었습니다.

### 4.3 레이아웃 안정화

- 작업 내용: 모든 이미지와 비디오 요소의 크기를 명시하고, 지연 로딩되는 요소들의 크기를 미리 지정하여 레이아웃 이동을 최소화했습니다.
- 개선 효과: CLS가 모바일에서 0.405에서 0으로, 데스크톱에서 0.513에서 0으로 크게 감소했습니다.

### 4.4 접근성 개선

- 작업 내용: 이미지 요소에 [alt] 속성 추가, 색상 대비율 조절, 제목 요소 내림차순으로 사용하도록 해 접근성을 개선했습니다.
- 개선 효과: 접근성 점수가 82점에서 100점으로 증가하여, 더 넓은 사용자층이 접근할 수 있도록 개선되었습니다.

### 4.5 검색 엔진 최적화

- 작업 내용: html 문서 내 메타 설명 추가, 이미지 요소에 [alt] 속성을 추가하여 검색 엔진 최적화에 대응하였습니다.
- 개선 효과: 검색 엔진 최적화 점수가 82점에서 100점으로 증가하여, 검색 엔진 순위가 향상될 수 있도록 개선되었습니다.

## 5. 향후 개선 계획

### 5.1 모바일 및 데스크톱 환경에서의 추가 최적화

- 개선 필요성: 성능은 최적화되었지만, 다양한 환경에서의 최적화와 새로운 요구 사항에 맞추어 추가적인 작업이 필요할 수 있습니다.
- 예정 작업: 리소스 최적화, CSS 및 JS 파일의 추가적인 미세 조정, 캐싱 전략의 개선 등을 계획하고 있습니다.

### 5.2 웹 접근성 및 사용자 경험 개선

- 개선 필요성: 웹 접근성과 사용자 경험을 더욱 향상시키기 위한 추가적인 최적화가 필요합니다.
- 예정 작업: 접근성 테스트를 통해 잠재적인 문제를 해결하고, 다양한 기기와 네트워크 환경에서의 성능을 지속적으로 모니터링할 예정입니다.

## 6. 결론

이번 성능 개선 작업을 통해 모바일과 데스크톱 환경 모두에서 성능 점수가 크게 향상 되었으며, 주요 지표들이 크게 개선되었습니다. 앞으로도 지속적인 모니터링과 최적화를 통해 최고의 사용자 경험을 제공할 수 있도록 노력할 것입니다.
