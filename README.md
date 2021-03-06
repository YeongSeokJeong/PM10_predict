# PM10_predict
## 목적
- 전날의 기상정보와 미세먼지 추이를 통한 정보 다음날 미세먼지 농도 예측
- 시간단위의 시계열 데이터를 사용한 정보 예측

## 데이터
- [기상청 기상예보데이터](https://data.kma.go.kr/cmmn/main.do)(서울시 종로구)
- [Air Korea 미세먼지 데이터](http://www.airkorea.or.kr/web)(서울시 종로구)

## 전처리
- 상관관계가 높은(서로 비슷한 의미를 가진) 데이터 제거
- 데이터 증폭을 위해 4시간 단위의 기상 데이터 분할

## 모델 
- LSTM + MLP

## 수정
```
initial commit(2019.12.13)	최초 커밋
modify code(2019.12.17)	        코드 수정(날짜 데이터 제거, 날짜 데이터 문자형 변환)
modify code(2019.12.23)         코드 수정(코드 오류 제거, 오버피팅을 막기위해 앞날의 데이터를 사용해 뒷날의 데이터 예측으로 변환)
adding new version(2020.1.3)	예측 ver 2 추가
modify readme(2019.1.6)			readme 추가
```
