### Box Model

img

**content** :

- width 너비
- height 높이

**padding** :

- 안쪽 여백
- content 와 border 사이의 공간
- 속기형
  `padding : top right bottom left;`

**border** :

- 테두리 굵기, 스타일, 색상 지정
  `border : 1px soild #000;`
- 꼭짓점 둥글게 만들기
  `border-radius : 50px;`
  `border-radius : 50%;`

**margin** :

- 바깥 여백
- 요소와 요소 사이의 간격
- 속기형
  `margin : top right bottom left;`

### Box Sizing

`box-sizing : content-box;`

- width, height를 content-box만의 사이즈로 지정됨
- 480\*480 사이즈의 정사각형을 만들때, padding 값이 포함되어 만들어짐.

`box-sizing : border-box;`

- border까지 포함하여 사이즈 지정됨

### Box Type

| Block | Inline | Inline Block | Flex |
| ----- | ------ | ------------ | ---- |

```
display : block;
display : inline;
display : inline block;
display : flex;
```

**block** :

- block은 자기 옆으로 다른 요소가 올 수 없도록 '길막'을 함
- block에 따로 width 지정하지 않을 시 부모 content-box의 100%
- width를 지정한 경우 남는 공간은 margin으로 채움 (부모width:1000px > width:400px, margin:600px)
- 따로 height를 지정하지 않은 경우 자식 요소 height의 합 = 부모 height
- border, padding, width, height, margin … 사용가능

**inline** :

- width, height, padding-top, padding-bottom, border-top, border-bottom, margin-top, margin-bottom … 사용불가
- padding-left, padding-right, border-left, border-right, margin-left, margin-right … 사용가능

**inline block** :

- inline과 block의 장점을 합침
