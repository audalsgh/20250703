# 9일차

## 1. numpy 어레이 복습
7월 3일 진도에 대한 문서 링크<br>
https://docs.google.com/document/d/17Avhfbh0q_K7FgLGbhBY_yvD3xCIdlAfVIRJUAP-lFU/edit?tab=t.0

*실무에서는 ROI 영역 추출을 위해, 인덱싱과 슬라이싱이 굉장히 많이 쓰인다.<br>
*Shape를 잘해야 메모리 효율성이 달라지고, 실제 영상은 노이즈가 끼고 여러 각도로 촬영되기에 필터와 데이터 증강(augmentation)을 해줘야한다. 
![image](https://github.com/user-attachments/assets/73cb4d2f-32ce-4156-bf55-ec371adfd7e2)

1. numpy가 무엇인지 기초 개념에 대한 애니메이션이 담긴 링크<br>
https://claude.ai/public/artifacts/0594c0ae-662a-4c1b-b29f-16dc69aff934
2. 배열 생성 및 인덱싱을 해보는 애니메이션이 담긴 링크<br>
https://claude.ai/public/artifacts/6accf154-ceb5-470a-b2e2-543df2d49b4a
3. 슬라이싱, 배열 연산을 해보는 애니메이션이 담긴 링크<br>
https://claude.ai/public/artifacts/fdea1f0a-439f-47d8-b954-956f34693a2e
4. Shape & Reshape 개념에 대한 애니메이션이 담긴 링크<br>
https://claude.ai/public/artifacts/e9e50b3f-cd6a-4a15-8858-3a84f0b4bb36
5. 브로드캐스팅 애니메이션이 담긴 링크<br>
https://claude.ai/public/artifacts/1e559e5e-1a60-4c8f-8971-69d9d00581ae
6. numpy로 자율주행 및 gps 계산을 하는 애니메이션과 코드<br>
https://claude.ai/public/artifacts/b16c6b7d-4afc-46ab-bd09-778bcd3bb149
![image](https://github.com/user-attachments/assets/a7c973d6-d4b9-429a-8b57-7e4baed004eb)

## 2. matplotlib 공부
colab에 작성한 w3schools 코드들 깃허브에 정리하여 이메일로 제출.
- (0703_python_matplotlib.ipynb)
  ### 몰랐던 개념들 정리.
- 함수 호출 시 a=1처럼 매개변수 이름을 함께 적어 넘기는 방식을 "키워드 인자(keyword argument)"라 부름.
  ```python
  # 키워드 인자 방식으로 plt.plot() 옵션을 주기에 순서는 상관없다.
  plt.plot(x, y, ls = '-', color='red')
  plt.plot(x, y, color='red', marker='*', ls = ':', lw =0.5, x, y)
  ```
- (반대 개념은 위치만으로 넘기는 방식인 "위치 인자(positional argument)")
- Matplotlib의 loc='best'는 “그래프 안에서 가장 빈 공간”을 찾아 범례를 배치하므로, 파이차트와는 어울리지 않는다.
```python
- plt.legend(
    loc='center left',            # bbox_to_anchor에서 지정한 점(왼쪽 중앙)에 범례의 'center'를 맞춘다
    bbox_to_anchor=(1.1, 0.5),    # (x, y) 튜플, x=1.1은 플롯 오른쪽 10%만큼 더 떨어진 위치를 의미, y=0.5는 중앙을 의미.
    title="Four Fruits:"
)
```
 
## 3. 0701 플로우 차트를 보고 코드를 짜보는 예제 9개 복습
- 나의 풀이 : https://github.com/audalsgh/20250701/blob/main/0701_python_flowchart_ex.ipynb
- 모범답안 : https://github.com/audalsgh/20250703/blob/main/0703_python_flowchart_ex_%EB%AA%A8%EB%B2%94%EB%8B%B5%EC%95%88.ipynb
- matplotlib 융합버전 : https://github.com/audalsgh/20250703/blob/main/0703_%EC%9E%90%EC%9C%A8%EC%A3%BC%ED%96%89%2Bmatplotlib_%EC%9C%B5%ED%95%A9_.ipynb
