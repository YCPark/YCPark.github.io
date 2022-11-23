---
title: "LISTAGG"
permalink: /posts/Oracle
categories: 
  - Oracle
toc: true
toc_sticky: true
toc_label: "Oracle"
tags:
  - Oracle
  - LISTAGG
---

## ROWS to COLUMN
> 여러행의 컬럼을 하나로 합치기 위하여   
`Oracle 11g R2`부터는 `LISTAGG()` 함수를 사용할 수 있습니다.   
   이전 버전의 경우 `XMLAGG()`, `WM_CONCAT()` 등의 함수를 사용했습니다.


매번 사용하는 함수가 아니라서 그런지 매번 사용법을 찾아가며   
해왔는데 이번 기회에 사용법을 정리해 두려 합니다.   
   

## Oralce Document - LISTAGG의 문법
---
![listagg_oracle_img](https://docs.oracle.com/cd/E11882_01/server.112/e41084/img/listagg.gif)

조금 복잡해 보일 수도 있는데 간단히 주로 쓰는 방식대로 하면 다음과 같습니다.

```
LISTAGG([column name], [delimiter]) 
    WITHIN GROUP(ORDER BY [column name])

LISTAGG([합칠 컬럼명], [구분자]) 
    WITHIN GROUP(ORDER BY [정령기준 컬럼명])
```

WITHIN GROUP 뒤로 OVER() 를 추가로 활용할 수 있습니다.

---

## 예제
```
WITH TAB AS
(
              SELECT '김철수' AS EMPL_NM FROM DUAL
    UNION ALL SELECT '김영희' FROM DUAL
    UNION ALL SELECT '홍길동' FROM DUAL
    UNION ALL SELECT '김유진' FROM DUAL
    UNION ALL SELECT '김동현' FROM DUAL
)
SELECT LISTAGG(EMPL_NM, ',') 
       WITHIN GROUP(ORDER BY EMPL_NM) AS VAL
FROM TAB A
-------------------------------------------------------
VAL
김동현,김영희,김유진,김철수,홍길동
```

## 참조
Oracle Document : <https://docs.oracle.com/cd/E11882_01/server.112/e41084/functions089.htm#SQLRF30030>   
LISTAGG : <https://gent.tistory.com/328>
{: .notice}