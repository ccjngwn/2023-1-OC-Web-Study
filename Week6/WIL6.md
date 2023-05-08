6주차에는 박스 모델과 fexible layout에 대해 배웠다.
- 박스 모델
    모든 html 요소는 박스 모양으로 구성되고, 이것을 박스 모델이라 부른다.
    1. content : 텍스트, 이미지 등이 들어있는 곳
    2. padding : content와 border 사이의 간격
    3. border : content와 padding을 감싸는 테두리
    4. margin : 테두리와 이웃하는 요소 사이의 간격
    margin과 padding은 시계방향으로 지정해 줄 수 있다.

- fexible layout
    flexbox를 사용하면 간단히 레이아웃 처리를 할 수 있다.
    이를 사용하기 위해선 html 부모 요소의 display 속성에 flex를 지정한다.
    
    .flex-container{
        display: flex;
    }
    
    - flex container 속성
    1. flex-direction
    flex-direction : row; - 요소가 좌에서 우로 수평 배치된다. default값
    flex-direction : row-reverse; - 요소가 우에서 좌로 수평 배치된다.
    flex-direction : column; - 요소가 위에서 아래로 수직 배치된다.
    flex-direction : column-reverse; - 요소가 아래에서 위로 수직 배치된다.

    2.flex-wrap
    flex-wrap : nowrap; - 요소가 1행에 배치된다. 각 flex item의 폭이 flex container에 들어갈 수 있는 크기로 축소된다.
    flex-wrap : wrap; - 각 flex item의 width 합계가 flex container의 width보다 큰 경우, 복수 행으로 배치한다. 좌우,위아래가 default 값
    flex-wrap : wrap-reverse; - wrap과 동일하나 아래에서 위로 배치된다.

    3. flex-flow
    flex-flow : <flex-direction> || <flex-wrap>; 위의 두 속성을 설정하기 위한 값

    4. justify-content
    justify-content : flex-start; - 시작을 좌측
    justify-content : flex-end; - 시작을 우측
    justify-content : center - 중앙에 정렬
    justify-content : space-between - 첫 번째와 마지막은 좌우 측면에 정렬되고 나머지는 균등한 간격으로 정렬된다.
    justify-content : space-around; - 모든 것이 균등한 간격으로 정렬된다.

    5. align-items
    align-items: stretch; - 꽉찬 높이를 갖는다
    align-items: flex-start; - cross start를 기준으로 정렬
    align-items: flex-end; - cross end를 기준으로 정렬