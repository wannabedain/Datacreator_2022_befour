## 2022 데이터 크리에이터 캠프

<img width="1277" alt="image" src="https://user-images.githubusercontent.com/91936267/226153107-0a593046-fb58-4432-87cd-9c4a03adc3c3.png">


## Mission 1 / 2
- EDA (클래스 별 분포 및 특성 확인)
  이미지 특성 값 width(가로), heigh(세로), pixel(픽셀) 추출
  이미지 채널을 BGR -> RGB로 변경
  각 이미지마다 픽셀 평균값 계산 
  -> Metadata 데이터 프레임 생성
  
  ### 학습 데이터의 불균형 존재  -> undersampling

  ### 일부 클래스의 픽셀 평균값이 낮음 -> 오염된 데이터가 들어갈 가능성이 있다고 판단
  #### AI 기반 영상 제거 : k-means 
    * 임의 차원 축소 / PCA 차원 축소 / AE 차원 축소
      * 평가 ( 실루엣 계수가 낮고, DBI ) 가 상대적으로 낮은 임의 차원 축소 & AE 차원 축소
      
## Mission 3
- 모델링 
  * CNN 구조
    : 하이퍼파라미터, 이미지 크기 설정
    
  <img width="639" alt="스크린샷 2023-03-19 오후 1 18 09" src="https://user-images.githubusercontent.com/91936267/226153361-bba333be-a805-4c7a-9de9-8370e2067412.png">
