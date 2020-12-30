# California housing prices prediction
- 데이터 변수
  
  - longitude : 경도
  - latitude: 위도
  - housing_median_age : 주택나이
  - total_rooms : 전체 방 수
  - total_bedrooms : 전체 침실 수
  - population : 인구
  - housefolds : 세대
  - median_income : 소득
  - ocean_proximity : 바다 근접도
- Linear regression

  -  Maximum Likelihood
      
      We will start with maximum likelihood estimation of the parameters 𝜽. In maximum likelihood estimation, we find the parameters 𝜽 that maximize the likelihood 𝑝(𝒚|𝑿,𝜽)=∑𝑝(𝑦𝑛|𝒙𝑛,𝜽).
      The maximum likelihood estimator is given by 
      𝜽=(X^T ∙ X)^−1 X^T ∙ y
      
      Define a linear regression model that is slightly more flexible : 
       𝑦 = Xaug^𝑇 ∙ 𝜽aug + 𝜖, Xaug=[1 𝒙], 𝜽aug = [𝜽0 𝜽1]^T
