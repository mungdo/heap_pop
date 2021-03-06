# heap_pop

공공데이터 시각화 프로젝트 : 어 느새 부터 heap.pop()은 안멋조.

---

## 프로젝트 :  코로나19 확산으로 재택근무가 늘었는가

1. 프로젝트 배경 : 
![스크린샷 2022-02-24 오후 2 44 48](https://user-images.githubusercontent.com/82261307/155633280-2c446f5d-708b-418c-8884-1086b6476c2e.png)
![스크린샷 2022-02-24 오후 2 41 44](https://user-images.githubusercontent.com/82261307/155633291-6eee9e28-64de-4853-b50b-b0d52911606e.png)
2. 프로젝트 목표 : 코로나 전후 출퇴근 교통 이용자 수, 사무실 공실률 등 다양한 지표를 통해 실제 재택근무 변화를 관찰하고자 한다.
3. 구성원 및 역할 : 강교철, 김순복, 권솔, 조성현, 안문주 
4. 데이터 수집 (18,19) (20,21)
    1. 출퇴근 시간대 교통 이용량 변화 분석을 통한 관찰 대상 지역 설정
        - [서울시 지하철 선별 역별 승하차 인원 정보](https://data.seoul.go.kr/dataList/OA-12914/S/1/datasetView.do#)
        
        - [서울시 버스노선별 정류장별 시간대별 승하차 인원 정보](http://data.seoul.go.kr/dataList/OA-12913/S/1/datasetView.do#)
    2. 관찰 대상 지역 공실률 분석
    - [서울시 오피스빌딩 임대료·공실률 및 수익률 (2013년 이후) 통계](https://data.seoul.go.kr/dataList/10613/S/2/datasetView.do)
    3. (추가예정)
5. 데이터 수집 및 분석 시스템 구축
6. 데이터 분석 및 시각화
    1. 전체 대중교통의 지역별 이동량 > 연도별 이동량
    2. 사무실 밀집 지역으로 이동하는 인구 (18,19 / 20,21)
    3. 전 후 차이 비교
    4. 사무실 밀집 지역 공실률 (18,19 / 20,21)
7. 분석을 통해 나온 인사이트
8. 개선사항 및 분석 결과

---

## 구성원

: 각자 이름 옆에 [branch](https://backlog.com/git-tutorial/kr/stepup/stepup2_2.html) 만들고 이름 작성해주세요.

* 강교철 : gyocheol
* 김순복 : sunbok
* 권솔 : sol
* 조성헌 : SeongHeon
* 안문주 : munju

---

## 파일 구성
```파일(폴더)명 : 설명```
> _heap_pop_ : 메인 프로젝트 폴더
> > _setting.py_ : 프로젝트 세팅 파일  
> > _views.py_ : 실행될 함수 생성  
> > _urls.py_ : 주소 이동시 실행될 함수 엮어줌  
> > ... (이외 파일들)
> 
> _templates_ : 탬플릿 폴더
> > _index.html_ : 메인 페이지 입니다. 무료 탬플릿 이용해서 만들었습니다.  
> > _원래인덱스.html_ : 기존 메인 페이지 입니다. (사용하지 않는 파일)  
> > __+ 각자 html 파일 생성해서 시각화 페이지 만들기__
> 
> ... (이외 파일들)

---

## 본인 html 페이지 완성 후 해야할 일

templates에 각자의 시각화 html 페이지 완성 후
1. _views.py_ 파일에 들어가서 함수 정의 
    ```python
    def 함수명(request): 
        return render(request, '본인이 만든 파일명.html')
   ```
2. _urls.py_ 파일에 들어가서 ```path('주소', views.함수명)``` 한 줄 추가
3. _index.html_ 파일에 들어가서 
    ```html
    <a class="list-group-item list-group-item-action list-group-item-light p-3" href="#!">...<... ```
    ```
    해당 a태그 href에 주소값 넣기
4. ```python manage.py runserver``` 실행 후 정상 실행 되는 경우에만 push
5. push 후 공유!

---
