# creditCalculatorWithSqlite

## 개발 step

    
1. DDL에서 scien_score 을 추가 
final String CREATE_SQL = "CREATE TABLE IF NOT EXISTS " + TABLE_NAME +" (  "
            + "  ID  INTEGER  PRIMARY KEY  AUTOINCREMENT, "
            + "  NAME     TEXT     NOT NULL,  "
            + "  KOR_SCORE     INTEGER     NOT NULL, "
            + "  ENG_SCORE     INTEGER     NOT NULL, "
            + "  MATH_SCORE     INTEGER     NOT NULL, "
            + "  SCIEN_SCORE    INTEGER     NOT NULL, "
            + "  GRADE     TEXT     NOT NULL, "
            + "  REG_DATE    TEXT     NOT NULL  )";
            
2. DML
final String INSERT_SQL = "INSERT INTO PERSON ( NAME, KOR_SCORE, ENG_SCORE, MATH_SCORE, SCIEN_SCORE, GRADE, REG_DATE) VALUES ( ?,?,?,?,?,?,?)";
    final String UPDATE_SQL = "UPDATE PERSON SET NAME = ?, KOR_SCORE = ?, ENG_SCORE = ?, MATH_SCORE = ?,SCIEN_SCORE = ?, GRADE = ? WHERE ID = ?";
    final String DELETE_SQL = "DELETE FROM PERSON WHERE ID = ? ";
            
            
            
       
 
  ## 실행 결과
  
![image](https://user-images.githubusercontent.com/86584041/123921056-92d0b900-d9c1-11eb-97e8-94044930f77e.png)


<img width="294" alt="스크린샷 2021-06-29 오후 10 53 48" src="https://user-images.githubusercontent.com/47955992/123809795-de855300-d92c-11eb-89bd-d2712e8e6196.png">
