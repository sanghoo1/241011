# grid

justify-items, justify-self
 모든 자식들의 내용물이 아닌 특정 자식의 내용물에 관여하고 싶을 때 사용하는 것이 self들이다.

앞서 items는 부모에서 지정해주었다면 이건 특정 자식에서 지정해주어야한다.


아이템이 많을 경우
grid-template-columns:repeat(22, 100px) ; 이런식으로 주면 컨텐츠가 넘친다.

grid-column: 1 / 4;
축약형
 1 / span 4  
 1번부터 시작해서 4칸차지

 repeat(auto-fill, minmax(100px, 1fr))
리피트 오토를 사용하면 넘치지 않으면서 그리드아이템들이 영역크기에 (1fr) 반응하여 적절히 채운다.
웹크기를 줄이면 영역크기가 줄어든다(90vw) 이때 1fr로 자동조절이 되게 하며 최소크기가 100px만큼까지만 줄어든다.
넘치지않게 자동 줄바꿈이 일어난다

웹크기를 늘리면 영역크기가 늘어난다. 1fr로 자동조절로 늘어나며
 계속 늘리면 원본크기를 유지하려고해서 여백이 생긴다.
 repeat(auto-fill, minmax(100px, 1fr)) 이 구조는 외우는 게 좋다.