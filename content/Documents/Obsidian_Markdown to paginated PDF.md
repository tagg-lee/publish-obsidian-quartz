---
created: 2023-10-18
---
Type:: 
Up:: 
tags:: 

# 옵시디언 | md to PDF 페이지 나누기

### Question from 겨울
옵시디언 마크다운으로 pdf 문서를 만드는 과정에서, 페이지를 나눌 방법이 있을까요?

> # 1주차
> - ...
> 
>\---
> 
> # 2주차
> - ...

이렇게 쓰면 1주차와 2주차가 같은 페이지에 출력되는데 저걸 각각의 페이지로 출력되게 할수있는지가 궁금합니다.


### Answer from 엘프화가

> `<div style="page-break-after: always;"></div>`
> 위 코드를 필요한 곳에 넣으면 된다고 하네요. 테스트해보니 잘 되는 것 같습니다.
> 
> 출처는 Obsidian Forum입니다
> https://forum.obsidian.md/t/page-breaks-for-pdfs/13107