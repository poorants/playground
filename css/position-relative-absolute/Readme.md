# position

|  value   |                          content                           |           remark           |
| :------: | :--------------------------------------------------------: | :------------------------: |
|  static  |                      basic operation                       | dependent on parentdefault |
| absolute | the position is set in absolute coordinates in html sector |   independent of parent    |
|  fixed   |   set the absolute position in the only displayed screen   |   independent of parent    |
| relative |  setting a position relative to the position it should be  |    dependent on parent     |
|  sticky  |                                                            |    dependent on parent     |


- 객체 속성에 relative가 선언 된 객체는 parent object가 된다. 
- 예외적으로 body tab는 기본적으로 relative 속성을 가지고 있다. 
- absolute는 html 구조 상 parent object에 해당하는 객체들 중 relative 속성을 가지고 있는 객체로부터의 상대 경로를 가진다. 
- 다중 relative 속성이 존재하면 제일 가까운 parent object(position: relative) 기준으로 움직인다. 
- 
