# Orpheus Music
react를 이용한 뮤직 플레이어

1. 제작 목적
생활코딩 html부터 react 수업까지 모두 다 수강하였지만 크게 와닿지 않았기에,
활용할 주제를 탐색하였습니다.

그중에서도 뮤직 플레이어가 눈에 들어왔습니다.
react의 생성, 업데이트 기능(useState, useEffect).. 
이런 것들을 다 써볼 수 있을 거 같아서 한번 만들어보았습니다.

2. 프로젝트 명칭
"디오니소스님 늦어서 죄송합니다"
이 밈이 너무도 맘에 들어, Orpheus라고 했습니다. 간단하죠?

3. 디자인
처음에는 Youtube Music의 디자인을 차용하려고 했습니다.
검정, 회색, 햐양 깔끔한 조합이 맘에 들었으나,

제가 생각한 Orpheus의 느낌은 받지 못했습니다.

일렉하프를 미친듯이 연주하는(?) 그런 느낌을 줄 수는 없을 거 같아,
분홍색 계열의 그라데이션을 넣어보았습니다.

uiGradients 같은 그라데이션을 추천해주는 사이트가 있어서 아주 좋더군요 ㅎㅎ

4. 코드
(추후 추가 예정)

5. 어려웠던 점

web audio api 코드가 작동하지 않아 힘들었습니다.
오디오 비주얼라이징 기능을 쪼오끔 배운 p5.js와 연계하고 싶었는데 할 수가 없었습니다.

// 오디오 요소를 얻습니다
const audioElement = document.querySelector('audio');
// 오디오 요소를 오디오 컨텍스트에 전달합니다
const track = audioContext.createMediaElementSource(audioElement);

이 코드가 HTMLAudioContext 타입이 아니라는 에러와 함께 떠서 골머리를 앓았습니다.
<script> 태그가 <body> 밖에 있어야 한다... 등등 여러 답변을 보았지만
문제가 해결되지가 않았습니다.

결국에는 다른 분이 만들어주신 audio visualizer module를 써서 해결을 하였지만 아쉬울 따름이네요...
