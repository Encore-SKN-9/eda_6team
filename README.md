## SKN09-EDA-6Team

**SK Networks AI Camp 9기**

**개발기간: 25.01.15 - 25.01.20**



## 1. Introduction Team (팀 소개)

### 팀명: SS (ShoeScope)

#### **팀원**

| 이름       | GitHub ID      |
| ---------- | -------------- |
| 윤 환     | [@MNYH](https://github.com/MNYH)
| 이세진     | [@tpwls9494](https://github.com/tpwls9494)
| 이윤재     | [@dadambi116](https://github.com/dadambi116)
| 조이현     | [@SIQRIT](https://github.com/SIQRIT)



## 2. Introduction Project (프로젝트 개요)

### **프로젝트명**: 경쟁 브랜드 제품 비교 분석

**소개**
- 브랜드, 가격, 할인가격, 인기순위의 4가지 분석 관점을 통해 나이키와 아디다스 제품의 관계를 비교분석하며, 각 분석 관점의 시각화 자료를 통해 차이점을 확인하고자 합니다.

**배경**
- 대표적인 신발 브랜드 하면 떠오르는 명백한 브랜드는 아디다스와 나이키입니다. 두 거대 기업이 큰 시가총액과 시장 점유율을 가지고 정상에 오르기 위해 경쟁하면서 어느 브랜드의 제품이 더 좋은가 끊임없는 논쟁거리가 되고 있습니다. 따라서, 수많은 제품들이 쏟아지며 소비자의 선택을 도와줄 수 있는 지표가 필요해졌습니다.

**목표**
- 경쟁 브랜드간 신발 제품들에 대한 다중 관점 분석 및 최적의 제품 선택방법을 도출합니다.



## 3. EDA Processing (EDA 진행과정)
1. 데이터 수집 및 선정
2. 데이터 전처리 (팀 공용 데이터)
3. 파트별 분배 후 분석 및 시각화
4. 분석 데이터 코드 조합
5. 문제점 보완 및 개선
6. 결론 및 인사이트 도출

---

## 4-1. 데이터 수집 및 선정

![nike_vs_adidas_dataset_cover](https://github.com/user-attachments/assets/42c3d8db-6724-42db-a2cb-0d38e2ea36a7)
![image](https://github.com/user-attachments/assets/e5b23076-7cef-4462-b2e7-f07610fed3b7)



## 4-2. 데이터 전처리 (팀 공용 데이터)

![image](https://github.com/user-attachments/assets/90de427e-b57c-4a7a-9114-d6b170f05f6a)
![image](https://github.com/user-attachments/assets/33064dfd-5320-46b9-a6c0-91190f161cea)
![image](https://github.com/user-attachments/assets/5d014d0d-ff62-4553-915a-81a5db0209db)
![image](https://github.com/user-attachments/assets/6c5a6ba0-21b9-46c1-8d67-3c4b57e82425)
![image](https://github.com/user-attachments/assets/e3e1e831-434d-487c-a55d-36411652b4f7)
![image](https://github.com/user-attachments/assets/d14878f4-0688-4903-b631-750a1ffd5176)
![image](https://github.com/user-attachments/assets/4c4b36d6-4bba-4b67-ad8a-7c680f1532be)
![image](https://github.com/user-attachments/assets/a599f975-97b5-449f-8069-2ea4f28897ac)
![image](https://github.com/user-attachments/assets/c3407945-a1fe-4871-8ce0-c399eab2d15a)



## 4-3. 파트별 분배 - 1) 우선분석

1. 가상의 페르소나 고객 2인을 설정
2. 고객 2인에 대한 요구사항을 정리
3. 데이터셋을 4가지 파트로 분배
4. 분배한 파트를 기준점으로 우선분석 시작
5. 팀원 모두 동일한 요구사항에 도달



## 4-4. 파트별 분배 - 2) 시각화

### 4-4-1. 분석1: 브랜드별 (진행자: 윤 환)

### 분석방향 설정
- 소비자의 입장에서 만약 아이쇼핑하려고 브랜드를 선택할 때, 무엇을 보고 선택하는가?
  1. 신발 이미지를 보거나 품명을 봐서 쇼핑을 진행한다.
  2. 찜해놓은 게 있다면 할인율을 보고 결정한다.
     - 이미지 (데이터셋에 존재하지 않음)
     - 품명 (분석 가능)
       - adidas는 브랜드가 4개로 분류되어, adidas 하나로 통합 시킴.
       - 각 브랜드별 데이터 추출 후, txt 파일로 저장
         - txt 데이터 육안으로 확인 후, 대중적인 품명 종류 5개 선정
         - 품명 종류에도 서로 겹치는 품명이 있어 분류 작업 진행.
           - (ex) air, zoom, jordan 분류했다면 air jordan, air zoom 이런식으로 제품명이 겹침.
         - 분류 후, 데이터 개수 확인 완료
         - pie chart 시각화 완료 
     - 할인 (분석 가능)
       - adidas, nike 각 브랜드별 할인 bar 차트로 구현 완료.
         - nike 할인 없음.
           - Listing Price(표시 가격)과 Sale Price(세일 가격) 다른게 있음.
           - 할인율이 적용이 안됨.
           - ※ discount(할인) 데이터에 대한 box plot 시각화.


- 각 브랜드 품명 분류
![shoes_data](https://github.com/user-attachments/assets/c0519dfa-9e53-40f1-91de-cd7bdc1fe4ee)


- 각 브랜드 할인율  
![discount_data](https://github.com/user-attachments/assets/6873393b-c102-4666-af7b-aa212a42a2b3)


- 각 브랜드 box 할인율  
![discount_box_data](https://github.com/user-attachments/assets/af19bede-e25f-444d-8de8-c5aa2a67fe19)




### 분석1 결과 및 인사이트 도출
- (TO DO)



### 4-4-2. 분석2: 가격별 (진행자: 이세진)

### 분석방향 설정
- 사람들이 신발의 가격과 함께 가장 중요하게 보는 것은 어느 것이 인기가 있는가이다.
    - 먼저 무슨 신발이 있는지가 제일 궁금할것이고,
    - 무슨 신발이 어느정도 있는지 확인한 후에는
    - 어떤 신발이 인기가 있고 그 가격이 얼마인지 확인을 할것이다.
        - 그에 따라 가장 잘 나가는 제품
        - 평점이 높은 제품
        - 리뷰가 많은 제품
        - 각 가격별로 나누어 top5, top10인 데이터를 추출해서 시각화 자료로 나타냈다.


- 카운트, 가격별 총 계수
![image](https://github.com/user-attachments/assets/)

- 가격대로 범위를 나눈 카운트 수
![image](https://github.com/user-attachments/assets/)

- 사람들이 많이 산 제품 top5
![image](https://github.com/user-attachments/assets/)

- 사람들이 많이 산 제품의 가격 top5
![image](https://github.com/user-attachments/assets/)

- 평점이 높은 제품 top5
![image](https://github.com/user-attachments/assets/)

- 평점이 높은 제품의 가격 top5
![image](https://github.com/user-attachments/assets/)

- 리뷰가 많은 제품 top5
![image](https://github.com/user-attachments/assets/)

- 리뷰가 많은 제품의 가격 top5
![image](https://github.com/user-attachments/assets/)
  

### 분석2 결과 및 인사이트 도출
- 각 가격대별로 나눈 결과
- 전체적으로 나이키가 아디다스보다 1.5배 가량 비싼 추세를 보이며,
  - 사람들이 많이 사는 품목 top5,
  - 리뷰별 순위 top10 는 나이키가 조금 더 가격대가 높았고
  - 별점별 순위 top10은 비슷한 추이를 보였다.
- 따라서, 가격을 신경쓴다면 아디다스를 고른다는 인사이트를 도출해낼 수 있다.



### 4-4-3. 분석3: 할인가격별 (진행자: 이윤재)
### 분석방향 설정
- 가격에서 함께 고려하는 요소 중 하나는 세일 가격이다.
  	- 단순히 세일 가격이 높다고 해서 그 신발을 선택하는 것이 아니라
  	- 리뷰나 평점 역시도 신발을 선택하는 기준에 영향을 미칠 것이다.
  	- 세일 가격이 높은 제품을 브랜드별 5개씩 10개를 선정해 시각화 자료를 보여준다
 
  	- 브랜드별 세일 가격의 범위
  	- 리뷰에 따른 브랜드별 상위 5개 제품의 세일가격
  	- 평점에 따른 브랜드별 상위 5개 제품의 세일가격
  	
- 브랜드별 세일 가격의 범위

![sale_price_scope](https://github.com/user-attachments/assets/e94bffd7-c5c3-4087-ac29-5f74f4eb2120)

- 리뷰에 따른 브랜드별 상위 5개 제품의 세일가격
![SalePrice_Reviews](https://github.com/user-attachments/assets/426547e0-5bb3-4be3-90e7-9c0bb0cc42db)


- 평점에 따른 브랜드별 상위 5개 제품의 세일가격
![SalePrice_Rating](https://github.com/user-attachments/assets/db850d9f-4365-49b9-b1c1-011c382e4155)



### 분석3 결과 및 인사이트 도출
- 결론
1. Sale Price 범위를 무조건적인 1순위로 본다면 Nike를 선택할 것이다.

2. nike의 상위 5개 제품을 리뷰 또는 평점을 기반으로 선택을 한다면,

    리뷰 수를 우선하는 경우, Nike 상위 5개 제품 모두 큰 차이가 없으므로 '용도별'과 같은 또 다른 기준을 적용하여 제품을 선택할 수 있다. 

    평점 우선시, 'Nike mercurial superfly 7 elite mds fg'의 수치가 앞도적으로 높은 편이므로 이를 선택한다는 결론에 도출했다.



### 4-4-4. 분석4: 인기순위별 (진행자: 조이현)

### 분석방향 설정
- 대체로 평점이 높으면 인기가 좋아서 리뷰가 많이 달릴 것이다.
- 그러나 평점만 높다고 반드시 인기가 좋은 것은 아니다.
- 리뷰도 악성리뷰가 많은 경우가 있을 수 있다.
- 따라서 메인 조건을 평점으로, 서브 조건을 리뷰로 건다.
    - 따라서 제품명과 판매량에 대한 groupby를 사용하여 1차 필터 적용
    - '제품명당 판매량'에 평점 내림차순 적용
        - 평점당 상위 10개 제품 시각화
        - '제품명당 판매량'과 평점간의 상관관계 시각화
    - '제품명당 판매량'에 리뷰 내림차순 적용
        - 리뷰수 상위 10개 제품 시각화
        - '제품명당 판매량'과 리뷰간의 상관관계 시각화

![image](https://github.com/user-attachments/assets/34a2801c-d5e5-4886-9f30-b937de4888ec)
![image](https://github.com/user-attachments/assets/283c8b25-de6e-4ff4-ae47-de84da6fbbf8)
![image](https://github.com/user-attachments/assets/25fed7df-1e06-42b3-a8ae-ac45dfba1791)
![image](https://github.com/user-attachments/assets/a72e82db-509f-401c-94cd-60338aadb27b)
![image](https://github.com/user-attachments/assets/3060da22-1de2-4bdf-bdeb-4585ed45b118)
![image](https://github.com/user-attachments/assets/3f248514-3162-47f8-9248-fd5e539ab4e5)
![image](https://github.com/user-attachments/assets/d4164619-47fb-4a8c-8e6e-2733f56870d4)
![image](https://github.com/user-attachments/assets/791bb270-1f73-4153-96a1-c17e34d47a4a)
![image](https://github.com/user-attachments/assets/750bd024-3a1d-4f6e-860d-ca676cae000b)
![image](https://github.com/user-attachments/assets/718e2cbe-2dfc-471d-83d3-3e449ac14026)
![image](https://github.com/user-attachments/assets/eef349c8-fa28-4c40-8ac5-8a879c710cef)



### 분석4 결과 및 인사이트 도출

- 평점과 리뷰의 히트맵 상관계수를 근거로 분석방향 설정에 대한 논리적 가설에 오류를 발견할 수 있었다. 따라서, 해당 오류를 수정하고 평점을 기준으로 한 평균 리뷰수를 통해 소비자가 원하는 제품 추천을 할 수 있게 되었다.



## 4-5. EDA 결론

(TO DO)

---

## 5. 팀원 한 줄 회고 🌈

- **윤 환**: 데이터 처리와 시각화를 통해 인사이트를 시각적으로 명확히 전달할 수 있었던 과정에서, 데이터의 가공과 표현의 중요성을 다시금 깨닫게 되었다.
- **이세진**: 데이터 전처리 과정에서 컬럼을 추가하거나 제거하는 작업을 직접 수행하며, 데이터 처리 방식에 따라 분석 결과가 크게 달라질 수 있다는 것을 실제로 경험하고 배웠다.
- **이윤재**: 데이터 분석의 기준을 어떻게 잡느냐에 따라 데이터 분석의 결과를 다양하게 낼 수 있음을 알게 되었다. 
- **조이현**: 데이터 분석 방향에 따른 결과의 차이가 유의미하게 날 수 있음을 발견했다. 또한 히트맵 상관계수 시각화를 근거로 기존에 설정했던 분석방향을 개선하는데 도움이 되었다.
