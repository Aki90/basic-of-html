## VIDEO, SOURCE, TRACK 요소
- VIDEO 요소는 동영상을 불러올 때 사용하는 요소입니다.
    - VIDEO 코덱에 따라서 어떤 브라우저에서는 지원하고, 어떤 브라우저에서는 지원하지 않을 수 있습니다.
    - 브라우저의 코덱 지원율을 잘 체크하시길 바랍니다.
- 공통으로 지원하는 속성이 있습니다.
    - SRC 속성을 이용해서 리소스의 경로를 지정합니다.
    - PRELOAD 속성을 이용해서 사전 로드 여부를 결정합니다.
    - CONTROLS 속성을 이용해서 브라우저 기본 컨트롤을 보여줄 지 결정합니다.
    - AUTOPLAY 속성을 사용해서 자동 재생 여부를 체크할 수 있습니다.
      - 웹 접근성 이슈로 인해 자동 재생을 사용할 경우에는 MUTED 속성을 사용해 음소거를 해둔 상태로 재생해야합니다.
- VIDEO는 그 특성상 더 많은 속성을 지원합니다.
    - PLAYSINLINE 속성은 모바일 브라우저에서 비디오가 페이지 내에서 재생되게 합니다.
    - POSTER 속성은 썸네일로 사용할 이미지를 지정할 수 있게 해줍니다.
- VIDEO에서 TRACK 요소를 사용하여 자막을 추가할 수 있습니다.
    - TRACK 요소에서 사용하는 표준 자막 포맷은 WEBVTT 입니다.

## AUDIO, SOURCE 요소
- AUDIO 요소는 오디오를 불러올 때 사용하는 요소입니다.
  - AUDIO 코덱에 따라 지원율이 다릅니다.
- AUDIO에서 지원하는 속성이 있습니다.
  - SRC 속성을 이용해서 리소스의 경로를 지정합니다.
  - PRELOAD 속성을 이용해서 사전 로드 여부를 결정합니다.
  - CONTROLS 속성을 이용해서 브라우저 기본 컨트롤을 보여줄 지 결정합니다.
  - AUTOPLAY 속성을 사용해서 자동 재생 여부를 체크할 수 있습니다.
    - 웹 접근성 이슈로 인해 자동 재생을 사용할 경우에는 MUTED 속성을 사용해 음소거를 해둔 상태로 재생해야합니다.

## IFRAME 요소
- IFRAME 요소는 외부 HTML 문서를 내 HTML 문서에 가져올 때 사용합니다.
- 다양한 용법이 존재하지만 가장 대중적으로 사용하는 건 YouTube, Facebook 등을 내 페이지 내에 Embed 할 때 사용합니다.
- 페이지 내부에서 다른 페이지를 불러올 때,
  - 내가 개발한 페이지를 페이지 내에서 IFRAME을 이용해 불러오는 건 불필요한 렌더링 비용을 유도하기 때문에 추천하지 않습니다.
  - 페이지 내에 SANDBOX 형태로 다양한 페이지를 구성해야할 때는 유용할 수 있습니다.
