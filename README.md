# creditCalculatorWithSqlite

   
  ## 개발방법: 

    
1. DDL에서 "scien_score" 테이블 을 추가 
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

- 데이터 추가 쿼리 ( scien_score 추가) 
"INSERT INTO PERSON ( NAME, KOR_SCORE, ENG_SCORE, MATH_SCORE, SCIEN_SCORE, GRADE, REG_DATE) VALUES ( ?,?,?,?,?,?,?)";
- 데이터 수정 쿼리 (SCIEN_SCORE 추가) 
"UPDATE PERSON SET NAME = ?, KOR_SCORE = ?, ENG_SCORE = ?, MATH_SCORE = ?,SCIEN_SCORE = ?, GRADE = ? WHERE ID = ?"; 
- 데이터 삭제 쿼리 
DELETE FROM PERSON WHERE ID = ? ";
            
       
 
  ## 실행 결과
  
1.메뉴
![image](https://user-images.githubusercontent.com/86584041/124346217-9d38c000-dc18-11eb-9e30-eb76ffe3dd96.png)

2.CRUD 기능
- read
![image](https://user-images.githubusercontent.com/86584041/124346256-ceb18b80-dc18-11eb-88e9-0267e02a5ce7.png)

- update 
전
![image](https://user-images.githubusercontent.com/86584041/124346291-f1dc3b00-dc18-11eb-9a64-22e34a837f2c.png)


후
![image](https://user-images.githubusercontent.com/86584041/124346300-fb65a300-dc18-11eb-8c47-a882b716149e.png)

- delete
![image](https://user-images.githubusercontent.com/86584041/124346313-0a4c5580-dc19-11eb-8b79-8c76bf08b4a0.png)

결과  :
![image](https://user-images.githubusercontent.com/86584041/124346322-146e5400-dc19-11eb-9c01-3ec0d30ff55a.png)



- 검색 
-![image](https://user-images.githubusercontent.com/86584041/124346336-29e37e00-dc19-11eb-97c0-8bebd1df6a04.png)

3.파일 불러오기
![image](https://user-images.githubusercontent.com/86584041/124346386-75962780-dc19-11eb-8d2d-124bb836e032.png)



4. 파일 저장하기 
![image](https://user-images.githubusercontent.com/86584041/124346369-5ac3b300-dc19-11eb-88f9-a304dc9908d0.png)

