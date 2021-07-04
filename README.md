# creditCalculatorWithSqlite

    
## >>> Customizing 
<br/><br/>


### DDL에서 "scien_score" 테이블 을 추가 
final String CREATE_SQL = "CREATE TABLE IF NOT EXISTS " + TABLE_NAME +" (  "
            + "  ID  INTEGER  PRIMARY KEY  AUTOINCREMENT, "
            + "  NAME     TEXT     NOT NULL,  "
            + "  KOR_SCORE     INTEGER     NOT NULL, "
            + "  ENG_SCORE     INTEGER     NOT NULL, "
            + "  MATH_SCORE     INTEGER     NOT NULL, "
            + "  SCIEN_SCORE    INTEGER     NOT NULL, "
            + "  GRADE     TEXT     NOT NULL, "
            + "  REG_DATE    TEXT     NOT NULL  )";
            
            
<br/><br/>
## DML

- 데이터 추가 쿼리 ( scien_score 추가) 
"INSERT INTO PERSON ( NAME, KOR_SCORE, ENG_SCORE, MATH_SCORE, SCIEN_SCORE, GRADE, REG_DATE) VALUES ( ?,?,?,?,?,?,?)";
- 데이터 수정 쿼리 (SCIEN_SCORE 추가) 
"UPDATE PERSON SET NAME = ?, KOR_SCORE = ?, ENG_SCORE = ?, MATH_SCORE = ?,SCIEN_SCORE = ?, GRADE = ? WHERE ID = ?"; 
- 데이터 삭제 쿼리 
DELETE FROM PERSON WHERE ID = ? ";
            
    <br/><br/>   
 
  # 실행 결과
  
## 1.메뉴<br/>
![image](https://user-images.githubusercontent.com/83248175/124380020-73090000-dcf5-11eb-97ed-fcadf277ad4c.png)
<br/><br/>

## 2.CRUD 기능<br/>
### 읽기 기능 <br/>
![image](https://user-images.githubusercontent.com/83248175/124380039-9af86380-dcf5-11eb-8bfd-024623a6511b.png)
<br/><br/>
update <br/>
### (update)수정 전
<br/>
![image](https://user-images.githubusercontent.com/83248175/124380084-cf6c1f80-dcf5-11eb-91d1-36195d881640.png)

<br/><br/>
### (update)수정 후<br/>
<br/>
![image](https://user-images.githubusercontent.com/83248175/124380115-f4f92900-dcf5-11eb-9f95-597edad23d68.png)
### delete
<br/>
![image](https://user-images.githubusercontent.com/83248175/124380129-0fcb9d80-dcf6-11eb-8a83-8183de25cb24.png)
<br/><br/>

### - 검색 <br/>
![image](https://user-images.githubusercontent.com/83248175/124380180-502b1b80-dcf6-11eb-9040-c33f311142f5.png)
<br/><br/>

## 3. 파일 저장하기<br/> 
![image](https://user-images.githubusercontent.com/83248175/124380205-6e911700-dcf6-11eb-84a3-268bd0d5a864.png)
<br/><br/>
