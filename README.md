# capston_design_CNN_malignant_project

1. 기간 : 2019.09~2019.12  

2. 기술스택 : python, json, numpy, matplot, tensorflow, keras  

3. 내용 : 피부암과 점을 CNN알고리즘을 통해 학습한 모델을 이용하여 classification.  
    1. 총 12162개의 데이터를 사용. 이 중 (training set을 10000개) + (test set을 2162개)
    2. jason형태의 메타데이터에서 나이, 성별, 부위, 피부암 유무 추출.
    3. jpg형태의 해당부위 사진을 PLT모듈을 이용하여 정형화.
    3. CNN알고리즘 적용
    4. 모델의 구조  
    ![구조](https://user-images.githubusercontent.com/50386280/78476121-4e834880-777f-11ea-95bf-22e6fd64ddf3.png)
    5. 결과  
        1. 그래프  
    ![그래프](https://user-images.githubusercontent.com/50386280/78477495-ae79ef00-777f-11ea-8b49-cf7ba379308e.png)  
        2. test set 정확도  
    ![결론](https://user-images.githubusercontent.com/50386280/78477874-c9e4fa00-777f-11ea-810d-c5c7274e2e48.png)


4. 파일설명
    [input file : folder.folder (대용량인 관계로 sample만) , output model : CNN_model.h5]  
    - input_data.ipynb : 전체 데이터 중 가용한 전체 데이터의 개수와 train set, test set으로 사용할 데이터를 overview.  
    - malignant.ipynb :  
        1. jpg데이터를 int형으로 변환
        2. jason 파일에서 피부암 유무 추출
        3. CNN알고리즘을 계층적 구조로 적용하여 모델링.
        4. 학습된 모델을 저장
        5. 결론 시각화
