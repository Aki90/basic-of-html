# HTML Grouping content
- 비슷한 의미를 가진 콘텐츠를 묶을 때 사용합니다.

## P 요소
- 문장을 의미합니다
## BLOCKQUOTE 요소
- 인용 블록를 의미합니다.
## OL, UL, LI 요소
- OL 요소는 순서 있는 목록, UL 요소는 순서 없는 목록을 나타냅니다.
- OL 요소는 주로 레시피, 사용설명서 등 순서에 따라 나타내야하는 목록을 나타낼 때 사용합니다.
- UL 요소는 네비게이션 메뉴, 버튼 메뉴 등 같은 의미를 가진 목록을 나타낼 때 사용합니다.
- OL, UL 요소의 자식 요소는 항상 LI 요소여야 합니다.
## MENU 요소
- 명시적으로 '클릭 가능한 버튼'을 포함하고 있는 목록을 의미합니다.
- MENU 요소의 자식 요소는 항상 LI 요소여야 합니다.
- 아직 브라우저 지원율이 낮으므로 사용에 유의하셔야 합니다.
```
<menu>
  <li><button type="button">복사하기</button></li>
  <li><button type="button">자르기</button></li>
  <li><button type="button">붙여넣기</button></li>
</menu>
```
## DL, DT, DD 요소
- DL 요소는 설명 목록을 나타내며, 제목 - 설명으로 이루어진 쌍을 관리합니다.
- DT 요소는 설명 목록에서 '설명하고자 하는 대상' 을 나타냅니다.
- DD 요소는 DT 요소에 이어서 '대상에 대한 설명' 을 나타냅니다.
- KEY : VALUE 구조라고 생각하시면 더 이해가 쉽습니다.
- DL 요소 내부에서 하나의 DT에 여러개의 DD를 사용할 수 있습니다.
  - 만약 여러 쌍의 DT와 DD를 사용하는 경우 DIV 요소를 사용해 그룹화할 수 있습니다.
    - 별도의 역할을 수행하지는 않지만, 추후 CSS를 넣거나 공통 속성을 넣을 때 유익합니다.
## FIGURE, FIGCAPTION 요소
- FIGURE 요소는 본문의 내용을 부연 설명하기 위해 사용하는 요소입니다.
- FIGCAPTION 요소와 함께 사용되며, 본문 중간에 삽입하여 부연 설명을 넣습니다.
- ASIDE 요소는 '연관되어있지만 독립된 콘텐츠'를 의미했다면, FIGURE 요소는 '연관된 콘텐츠' 자체를 의미합니다.
  - 즉 독립성을 보장하지 않아도 무관합니다.
- 이미지, 동영상, 오디오 등을 활용한 부연설명에 많이 사용됩니다.
## MAIN 요소
- MAIN 요소는 HTML 페이지 내에서 가장 중점이 되는 콘텐츠를 명시적으로 나타낼 때 사용합니다.
- 페이지 내에서 VISIBLE 상태인 MAIN 요소는 언제나 한 개여야 합니다.
- HTML 속성 중 hidden 을 사용하여 감추는 경우에는 여러개를 사용할 수도 있습니다.
  - JavaScript를 활용해 Router를 제어하는 경우 유용하게 사용할 수 있습니다.
## DIV 요소
- 명시적인 의미를 가지지 않으며, CSS 처리나 속성값 부여를 위해 여러 요소를 묶을 때 사용하는 요소입니다.
- HTML Living Standard 에서는 가장 마지막 수단으로 쓰라고 합니다.
  - 다른 요소가 충분히 DIV 역할을 수행할 수 있다면 해당 요소를 사용합니다.
  - IE 지원을 위해서 사용하는 경우가 있습니다.
- 실무에서 자주 쓰이기는 하지만 최근 저는 자주 쓰지 않는 요소 중 하나입니다.
- 다른 요소로 대체 가능할 지 만드시 체크한 후 사용하세요.