# HTML Sections
- Sections 카테고리에 포함되는 요소들은 페이지의 Outline을 명시적으로 생성할 때 사용합니다.
- 대부분의 요소가 Heading 요소를 필수로 합니다.

## Section, Article 요소
- Section, Article 요소는 제목 - 내용 관계를 형성할 때 특정 구역을 명확하게 분리시킬 때 사용합니다.
- Heading 요소만으로도 구역은 분리되지만 몇가지 문제가 생깁니다. => <u>article / section 과 함께 사용 권장</u>
  - 이 제목이 어느 콘텐츠까지 영향을 주는 지 알기 어렵습니다.
  - 제목의 아웃라인을 살펴보기 어렵습니다.
  - React, Angular, Vue 같은 프런트엔드 프레임워크를 사용하면, 파일이 분리되어서 더 이해하기 어렵습니다.

## section vs article
- article 요소는 article 요소 내부의 콘텐츠만으로도 '독립적인 콘텐츠'로 동작할 수 있을 때 사용하고,
- section 요소는 조금 더 '범용 목적으로 콘텐츠'를 감쌀 때 사용합니다.
- heading 요소를 사용하여 section 및 article 요소의 콘텐츠 범위를 명확하게 할 수 있으며,
- section, article 요소를 사용할 때 heading 요소를 반드시 작성하시기를 바랍니다.

## nav 요소
- nav 요소는 페이지 네비게이션 (탐색)을 생성할 때 사용하는 요소
- 주로 a 요소와 함께 사용됩니다.

## aside 요소
- aside 요소는 페이지 콘텐츠와 연관성은 있지만, 해당 콘텐츠와는 별개로 간주될 수 있는 콘텐츠를 의미합니다.
- 이런 섹션은 종종 페이지 콘텐츠의 사이드바로 보이게 하기도 하며, figure 요소와 함께 사용하기도 합니다.

## hgroup 요소
- hgroup 요소는 여러 개의 heading 요소를 그룹할 때 사용하며,
- 이 때 hgroup 외부에서는 hgroup 내부에서 가장 높은 레벨의 heading 요소를 따라갑니다.
  - hgroup 요소를 활용하여 제목, 부제목, 대체제목, 태그라인 같이
  - 여러 제목을 활용해야 하는 케이스를 처리할 수 있습니다.

## header, footer 요소
- header 요소는 보통 콘텐츠의 개요를 나타낼 때 사용하며,
- footer 요소는 보통 콘텐츠의 Summary나 작성자 등을 나타낼 때 사용합니다.

## Recap
HTML Sections는 페이지 전체의 outline을 생성하고,  
콘텐츠가 담고 있는 의미가 정확히 무엇인가에 대해서 명시적으로 표현하는 요소들입니다.

따라서 Sections를 잘 다루는 것만으로도 HTML에서 가장 큰 영역별 시맨틱을 구현할 수 있습니다.