


## thymeleaf - Spring combination



### 4 / 7 / 2024
#### html 일반 checkbox의 문제점 
 - html에서 일반 checkbox 사용시 on(체크됨)일 시 서버에 값을 true로 넘겨주지만
체크 안했을 시에는 그냥 null로 값을 아예 안넘겨준다.
- 스프링에서는 이를 방지하고자 html에서 hideen field를 둬서 "_ID"로 value="on"을 html내에 필드를 추가하여
서버에 넘겨주면 본래 checkbox/hidden의 값이 on/on 이면 true으로 인식, null/on일시 false로 인식하여 주는 기능이 있다.
- 결론은 이런 기능이 있다해도.. 여전히 매우 불편하다