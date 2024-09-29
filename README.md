
# 표/그림 객체 인식 데이터셋
 
## 개요
- The data for extracting metadata from PDF domestic papers.
- The data contains information in layout box extracted from each PDF paper with labels corresponding to metadata field types.
- The information in each layout box are unique code, text, coordinates(x0, y0, x1, y1) of box, width of box, height of box and font size.
- The file named as “train.txt” was constructed through the fully automatic inspection process. It contains a total of 5,241,746 labeled layout boxes for 295,306 papers in 503 journals. It was used as train set.
- The file named as “valid.txt” was developed through the manual inspection process by several annotators. It contains a total of 155,629 labeled layout boxes for 9,895 papers in 503 journals.
- The file named as “test.txt” was built through the manual inspection process. It contains a total of 159,925 labeled layout boxes for 10,119 papers in 503 journals. It was used as test set.

## 데이터 포맷(JPG, TXT)
|유형|설명|
|--|--|
|JPG|표/그림이 존재하는 연구보고서의 페이지를 이미지 파일로 변환|
|TXT|각 페이지에 존재하는 표, 그림, 캡션의 레이블 및 좌표 정보를 포함|

\<표, 그림, 캡션 레이블 및 좌표 정보 예\>
![docimage3](https://github.com/user-attachments/assets/0ea9aee9-9374-418e-9e78-52337161bd81)


## 데이터 통계
- 페이지(파일) 수: 9,124개
- 데이터셋 개수: 표: 7,096 그림: 107,30 표캡션: 6,799 그림캡션: 10,615
- 레이블 개수: 4 (0: 표, 1: 그림, 2: 표캡션, 3: 그림캡션)

## 데이터 구축방법
2021~2022년에 등록된 국가R&D보고서를 대상으로 이미지 추출 모델을 이용하여 1차로 표와 그림을 추출하고, 이후 어노테이터가 검증하는 방식으로 구축했다.

##  데이터 다운로드
http://doi.org/10.23057/71

## 라이선스
비영리 이용, 출처 표기, 재배포 금지
<br>※ 제공하는 데이터는 연구 수행 주체의 비공개 요청에 의해 일부 삭제가 될 수 있으며, 연구용으로만 사용해야 하며 재배포를 절대 금지함.
