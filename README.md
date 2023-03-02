# 수원대학교에서 진행한 문서 및 코드 저장소

## 1. [교내 경진대회] 국건영 데이터과학

- 문서 작성일 : 2023. 03. 02. 목요일
- 본 조사의 목적은 국민의 건강수준, 건강행태, 식품 및 영양섭취 실태에 대한 국가 단위의 대표성과 신뢰성을 갖춘 통계를 산출하고, 이를 통해 국민건강증진종합계획의 목표 설정 및 평가, 건강증진 프로그램 개발 등 보건정책의 기초자료로 활용하는 것이다.

### 1. 대회 참가 학생 소개 및 역할

- 팀 이름 : 수원대 질병 관리청
- 대회 참가 학생 소개 및 역할

|   학번   |  이름  |                                                                                                  역할                                                                                                  |
| :------: | :----: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
| 20516001 | 강서연 |                                             1. 데이터 시각화하기.<br>2. 모델링하기. <br> 3. Grid Search를 이용하여 의사결정트리 하이퍼 파라미터 튜닝하기.                                              |
| 20516008 | 김노정 | 1. [참고용] 조사자들의 전체 기본 정보 전처리 및 시각화 제작하기.<br>2. 데이터 전처리 및 시각화하기.<br>3. 최적의 모델 선택 및 시간 소요 그래프 제작 및 성능 점검하기. <br> 4. 의사결정트리 시각화하기. |
| 20516019 | 김시은 |                           1. 질병과 가구소득 관계 시각화하기.<br>2. 상관관계 분석하기.<br>3. k-means를 통해 영양 성분 클러스터링하기.<br>4. 평균값을 알아보고 pca 적용하기.                            |
| 20516053 | 성수빈 |                                                                               1. 데이터 시각화하기.<br>2. ppt 제작하기.                                                                                |

### 2. 대회 준비 진행 및 문제 해결 방식

1. 주제를 정하기 전에 전반적인 데이터의 경향을 알아보기 위하여 전체 칼럼에 대하여 전처리 및 시각화를 진행하였습니다. 칼럼은 환자의 기본 정보, 구체적인 검사, 식품 섭취 조사, 질병 유무로 크게 나눠서 진행하였습니다.
2. 주제는 가구 소득수준에 따른 남녀 연령별 영양 섭취 질병 예측 모델로 정하였습니다.
3. 해당 없음 (-1), 응답 안 함 또는 모름 (-2) 는 제거하였습니다.
4. 주제에 맞게 구체적으로 시각화를 진행하다 보니, 데이터의 불균형이 확인되었습니다. 표준화와 PCA 그리고 클러스터링을 이용하여 해결하기로 하였습니다.
5. Elbow curve를 이용하여 최적의 k를 찾았습니다. 그를 이용하여 필수 영양소 (탄, 단, 지)와 필수 영양소 이외의 영양소로 나누어서 각자 클러스터링을 진행하였습니다. (섭취량 적음, 섭취량 보통, 섭취량 많음으로 그룹화가 진행되었습니다.)
6. 필요한 칼럼을 선택하고 모델링을 진행하였습니다. 하이퍼 파라미터 튜닝 전에도 꽤 높은 정확도를 보였습니다.
7. 가장 좋은 모델을 선택한 뒤에 Grid Search를 이용하여 하이퍼 파라미터 튜닝을 진행한 뒤 해당 모델의 시각화를 진행하였습니다. 정확도가 훨씬 많이 올라갔습니다.
