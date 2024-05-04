## 이번 주차 내용
1) 누적막대 차트
---
2) 간트 차트
- 시간의 경과 또는 어떤 활동에 대한 기간을 표시하는 데 적합(ex 프로젝트의 수행 기간 등등)
- 즉 시계열적 요소가 있는 데이터를 나타내는 데 사용할 수 있다.
- DATEDIFF('단위', A, B) : A 차원과 B 차원의 날짜 차이를 단위로 환산해서 반환하는 함
---
3) 히스토그램
- 연속형 측정값을 기준으로, '구간' 차원을 만드는 데 사용할 수 있다
  - 즉 특정 구간에 얼마나 범주형 값들이 분포되어 있는지 살펴볼 수 있음
- fixed 함수 : {FIXED 차원 : 집게함수}
  - 지정된 차원만 사용해서 집계를 계산할 수 있다
    >> 여기서는 각 고객명의 첫 주문 일자와 두번째 주문 일자

- IIF 함수 : IFF(조건, A, B)
  -  조건이 맞으면 A를, 아니면 B를 반환함 + 알 수 없으면 세 번째 입력값 또는 NULL을 반환
- 측정값에서 구간차원 만들기 : 측정값 우클릭 -> 만들기 -> 구간차원 선택 -> 원하는 구간 차원 크기 입력
- NULL 값 처리하기 : 여기서는 재주문 없이 한 번만 구매한 고객들. 
  >> NULL을 없애고 싶으면 오른쪽 하단 1NULL 선택후, '데이터 필터링' 선택
- 막대 차트에서, 막대의 각 크기를 조절할 수도 있다
  >> 크기 마크 선택 -> 막대의 크기 '수동'으로 변경 -> 슬라이더로 조정
---

4) 이중 축 만들기(Dual Axis)
- 하나의 뷰에 이중으로 축을 사용함
- 복수 개의 값을 비교해서 보기 위한 경우 사용
  - 서로 동일한 마크를 사용할 수도 있고, 다른 마크를 사용할 수도 있음
- 또는, 뷰의 디자인을 위해서 사용되기도 함(도넛 차트 등)
- '축 동기화' 설정 유용하게 사용하기

---

5) 결합된 축 만들기(Combined Axis)
- 이중 축과 달리 하나의 축을 공유함
- 사실상 이중 축에서 축 동기화를 한 것이 결합된 축

  
## 실습 내용
태블로 퍼블릭 : https://public.tableau.com/app/profile/jongjin.kim/viz/3_17148441253460/Stateprofit?publish=yes
![연도별 카페인디카페인 profit 합계](https://github.com/ToBeWithYouPopcorn/24-1-Visualization-Study/assets/154731662/f96ace9c-46c1-4323-a299-b8ab52da7208)
![State별 평균 profit](https://github.com/ToBeWithYouPopcorn/24-1-Visualization-Study/assets/154731662/7ee73bbf-e4cb-4f76-ad63-dd261ef16342)

* 간트 차트를 시도해보고 싶었으나, 마땅한 시계열 데이터가 없어서 실패
* 대신 이중 축을 사용한 실습 진행

## 퍼블릭 태블로 추가 서치

https://public.tableau.com/app/profile/erikrettman/viz/RoundedProgressGanttCharts/RoundedProgressGantt
![Rounded Progress Gantt](https://github.com/ToBeWithYouPopcorn/24-1-Visualization-Study/assets/154731662/13a376cc-c14d-4cb4-a675-0af3aae785fd)

https://public.tableau.com/app/profile/technical.product.marketing/viz/GanttChartinTableau/ProjectManagement
![Project Management](https://github.com/ToBeWithYouPopcorn/24-1-Visualization-Study/assets/154731662/86aa0f92-d52e-464a-a1c5-d3ca9622020e)


- 간트 차트를 잘 나타낸 예시가 있어서 가져왔다
- 특히 두 번째 예시는 프로그램 진행 상황에 대한 내용을 간트 차트로 나타내 인상깊었음
