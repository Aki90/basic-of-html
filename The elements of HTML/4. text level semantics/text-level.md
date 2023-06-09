# Text-level semantics
- Text-level sematics는 HTML 문서 내에서 텍스트로 취급되는 요소들을 의미합니다.

## A 요소
- A 요소는 HTML 문서 내에서 Hyperlink를 생성할 때 사용합니다.
- Hyperlink란 다른 페이지로 이동할 때 사용하는 링크를 의미합니다.
- HTML 4.01 이나 XHTML 시절의 콘텐츠 모델로 인해 a 요소 내부에 block 요소를 넣지 못한다는 오해가 있습니다.
- HTML 5부터 콘텐츠 모델이 바뀌었기 때문에 표준에서 a 요소 내부에 block 요소를 넣을 수 있습니다.
  - 정확히는 content model에 따라 바뀐 것입니다.
- A 요소의 href 속성은 필수값이 아닙니다.  
  A 요소를 비활성화하고 싶다면 href 속성을 제외시킬 수 있습니다.
- A 요소에 target 속성을 사용해 페이지 이동을 어떻게 할 지 결정할 수 있습니다.
  - ```<a href="https://naver.com" target="_blank">네이버로 이동 (새창으로 이동)</a>```
- A 요소에 download 속성을 이용해 리소스를 다운로드 받게 할 수 있습니다.

## EM, STRONG 요소
- EM 요소와 STRONG 요소 모두 텍스트의 일부 영역을 강조하고 싶을 때 사용합니다.
- EM 요소가 단순한 강조라면, STRONG 요소는 필수 (반드시 읽어야 한다)에 더 가깝습니다.
- 따라서 강한 강조를 해야할 때는 STRONG, 일반 강조시에는 EM 요소를 활용하시기를 바랍니다.
  - 스크린 리더가 STRONG과 EM 요소를 읽어주는 억양이 약간 다릅니다.
- Heading 요소 내에서 일부 영역만 강조하고 싶을 때 STRONG 요소를 활용할 수 있습니다.
  - ```<h1>Chapter 1. <strong>HTML 시맨틱</strong></h1>```

## CITE, Q 요소
- CITE 요소와 Q 요소 모두 외부에서 가져온 콘텐츠를 명시하여 나타낼 때 사용합니다.
- CITE 요소는 저서, 출판물, 인물 등 사물에 대한 인용을 나타낼 때 사용합니다.
  - 출처에 가깝습니다.
- Q 요소는 인용구를 나타낼 때 사용합니다.
  - BLOCKQUTE가 인용 블록, Q가 인용구를 의미합니다.

## DFN, ABBR 요소
- DFN 요소는 이 페이지에서 최초로 정의된 용어를 정의할 때 사용합니다.
  - 전문 용어 등 쉽게 인지하기 어려운 용어를 정의할 때 사용합니다.
- ABBR 요소는 약어를 나타낼 때 사용합니다.
  - title 속성을 사용해 전체 명칭을 작성해줍니다.
- DFN 요소와 ABBR 요소를 반드시 함께 사용할 필요는 없습니다.

## CODE 요소
- CODE 요소는 문장 내에서 소스 코드를 표현하고 싶을 때 사용합니다.
  - [W3C Charactor Entity Code 정리](https://html.spec.whatwg.org/multipage/named-characters.html)

## SPAN 요소
- SPAN 요소는 특별한 의미를 가지고 있지는 않으며, 여러 텍스트 요소를 묶어서 표현하고자 할 때사용하는 요소입니다.
- DIV 요소와 용법이 유사하며, DIV와 마찬가지로 더 이상 사용할 요소가 없을 때 사용하는 요소입니다.
- 주로 속성을 넣거나, 스타일을 넣는 등의 동작으로 사용하게 됩니다.

## BR, WBR 요소
- BR 요소는 텍스트 내에서 줄바꿈을 일으키고 싶을 때 사용합니다.
  - 줄바꿈 문자가 하나 들어가는 것과 동일한 동작이며, HTML에서 줄바꿈을 구현하는 유일한 방법입니다.
- WBR 요소는 텍스트 내에서 줄바꿈을 일으키나, 텍스트 박스의 영역이 더 이상 한 줄로 보여줄 수 없을 때에만 줄바꿈 시킵니다.
  - 한줄로 보이던 콘텐츠를 특정한 케이스에만 두줄로 보이게 하고싶을 때 유용합니다.
  - CSS에서 word-break: keep-all 과 비슷한 동작입니다.