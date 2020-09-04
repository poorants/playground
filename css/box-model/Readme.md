# box-model

속성 : width, height, margin, padding, border, outline

## border-style

| value  |       content        |
| :----: | :------------------: |
| solid  |         실선         |
| dashed |       긴 점선        |
| dotted |         점선         |
| double |        2라인         |
| groove | 안쪽으로 들어간 라인 |
| inset  |  안쪽 그림자 스타일  |
| outset | 바깥쪽 그림자 스타일 |

## box-sizing

box 사이즈 선언 시 **600px** 크기의 박스를 만들고 싶을 때 **width** 옵션으로 600px 설정 후 margin, padding, border-width에 의해 설정 된 크기가 추가되어 최정적으로 사용하고자 했던 600px보다 더 큰 사이즈가 되버림. 

<br>

이 때 사용하는 옵션이 **box-sizing** 옵션임.

```css
div {
box-sizing: border-box;
}
```

|    value    |                                   content                                    | default |
| :---------: | :--------------------------------------------------------------------------: | :-----: |
| border-box  | width, height가 content, padding, border-width 값을 포함 **※ margin은 제외** |         |
| content-box |                    width, height가 content 영역에만 해당                     |    v    |

## border-radius
모서리 값을 둥글게 만들기 위한 옵션으로 사각형을 기준으로 **top-left**, **top-right**, **bottom-right**, **bottom-left** 네 꼭지점을 둥글게 표현한다. 
<br>
입력되는 값은 px 단위 또는 % 이며 50%가 width의 최대 값과 동일한 의미로 적용된다. **※ 50% 이상은 모두 동일한 모양**

|              value               |                           content                           |  etc  |
| :------------------------------: | :---------------------------------------------------------: | :---: |
|       border-radius: 30px        |                           **ALL**                           |       |
|     border-radius: 30px 0px      | **"top-left & bottom-right"** **"top-right & bottom-left"** |       |
|   border-radius: 30px 0px 10px   |     top-left **"top-right & bottom-left"** bottom-right     |       |
| border-radius: 30px 5px 30px 5px |         top-left top-right bottom-right bottom-left         |       |

## outline

- border를 감싸고 있는 라인
- border와 margin 사이에 위치
- border 안쪽에 위치하려면 '-' 값


# margin & padding 적용방법
margin과 padding은 값의 수에 따라 적용되는 위치가 다르다. 


|           value           |                content                |  etc  |
| :-----------------------: | :-----------------------------------: | :---: |
|       margin: 30px        |                **ALL**                |       |
|     margin: 30px 5px      | **"top & bottom"** **"right & left"** |       |
|   margin: 30px 5px 30px   |     top **"right & left"** bottom     |       |
| margin: 30px 5px 30px 5px |         top right bottom left         |       |