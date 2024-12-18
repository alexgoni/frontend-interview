## JavaScript만 사용하는 것과 비교해 TypeScript를 사용하는 이유에 대해 설명해 주세요.

JS는 동적 타입 언어로 런타임 싱 타입이 결정됩니다.

이 때문에 런타임 도중에 타입 에러가 발생하거나, 코드가 복잡해질수록 각각의 타입을 추적하기 어려워 생산성이 저하될 수 있습니다.

이를 해결하기 위해 JS의 슈퍼셋 개념인 TS가 등장했습니다.  
TS는 트랜스파일러로 JS가 실행되기 전 변수의 타입을 검사합니다.  
또한, 타입을 명시하는 것으로 코드 가독성을 높이고, 자동 완성을 통해 개발 생산성을 향상시킵니다.

## TypeScript의 동작 원리에 대해 설명해 주세요.

tsc는 작성된 ts 파일을 파싱하여 AST를 생성합니다.  
이 AST를 기반으로 타입 정보를 확인하고, 타입 체크를 수행합니다.  
타입에 문제가 없다면 이를 JS 코드로 변환합니다.

브라우저나 Node.js는 변환된 JS 코드를 가지고 다시 AST를 생성하고,  
AST를 가지고 바이트 코드로 변환해 실행합니다.
