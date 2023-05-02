# Sort | 정렬
데이터를 특정한 기준에 따라서 순서대로 나열하는 것
- 각 정렬 알고리즘의 시간복잡도를 비교하는데, **시간복잡도**에 대해 학습이 필요하신 분은 [여기](https://seen-young.tistory.com/46#c2)를 참고하세요

![image](https://gmlwjd9405.github.io/images/algorithm-quick-sort/sort-time-complexity.png)


<br>

# Sort 종류
- [버블 정렬(Bubble Sort)](#bubble-sort--버블-정렬)
- [선택 정렬(Selection Sort)](#selection-sort--선택-정렬)
- [삽입 정렬(Insertion Sort)](#insertion-sort--삽입-정렬)
- [퀵 정렬(Quick Sort)](#quick-sort--퀵-정렬)
- [병합 정렬(Merge Sort)](#merge-sort--병합-정렬)
- [계수 정렬(Counting Sort)](#counting-sort--계수-정렬)

<br>

- [Time Sort](#time-sort)




<br>

## Bubble Sort | 버블 정렬
시간복잡도 : O(N<sup>2</sup>)  

- 배열의 처음부터 끝까지 두 수(a, b)를 선택한 뒤 정렬되어 있지 않으면 두 수의 위치를 변경한다.
- [구현 코드 보러 가기](https://github.com/kseenyoung/coding-test-with-python/blob/main/정렬/Bubble%20Sort.py)

![1*0aPxBKrbMTVbF0UCI6gxZg](https://user-images.githubusercontent.com/65147869/233764423-1c701a84-bf4c-4f54-8624-44e10b455e80.gif)










<br>

## Selection Sort | 선택 정렬
시간복잡도 : O(N<sup>2</sup>)

- N + (N-1) + (N-2) + ... + 1 = N*(N-1)/2 (등차수열의 합 공식) 이므로 O(N<sup>2</sup>)
- 정렬되지 않은 데이터 중 가장 작은(큰) 수를 정렬된 수들 가장 뒤에 붙여가며 정렬한다.
- [구현 코드 보러 가기](https://github.com/kseenyoung/coding-test-with-python/blob/main/%EC%A0%95%EB%A0%AC/Selection%20Sort.py)

![img](https://user-images.githubusercontent.com/65147869/233765223-a2060a2a-7928-4a1e-8eea-d2429289c049.gif)







<br>

## Insertion Sort | 삽입 정렬
시간복잡도 : O(N<sup>2</sup>), Ω(N)

- **맨 처음 데이터와 정렬할 차례가 된 수의 앞은 항상 정렬**되어 있다고 가정하고 시작한다.  
- 데이터를 순서대로 방문하며 앞의 수가 본인보다 작을 때까지 앞 숫자와 순서를 바꾼다.
- [구현 코드 보러 가기](https://github.com/kseenyoung/coding-test-with-python/blob/main/%EC%A0%95%EB%A0%AC/Insertion%20Sort.py)

![1*JP-wURjwf4k23U2G3GNQDw](https://user-images.githubusercontent.com/65147869/233765261-fae8f5ae-c6a0-40b4-b7f9-6da056203e4a.gif)







<br>

## Quick Sort | 퀵 정렬
시간복잡도 : O(N<sup>2</sup>), Ω(NlogN)
- 가장 많이 사용되는 정렬 알고리즘. 프로그래밍 언어 정렬 라이브러리의 근간이기도 하다.
- 최악의 시간복잡도 O(N<sup>2</sup>)는 내림차순이나 올림차순으로 이미 정렬이 되어 있는 경우 발생
- 피벗 수를 하나 특정하여 정렬되지 않은 수들 중 **피벗보다 작은 숫자를 왼쪽**에서 부터 찾고 **피벗보다 큰 수를 오른쪽**에서 부터 찾는다.
- [구현 코드 보러 가기](https://github.com/kseenyoung/coding-test-with-python/blob/main/%EC%A0%95%EB%A0%AC/Quick%20Sort.py)

<br>

![image](https://user-images.githubusercontent.com/65147869/233765514-380d7b1e-8c6f-469a-aab2-caa4fc54e090.gif)






<br>

## Merge Sort | 병합 정렬
시간복잡도 : O(NlogN), Ω(NlogN)

![image-2](https://user-images.githubusercontent.com/65147869/233765535-17eb312f-beb8-4840-bd46-a2602dc80202.gif)






<br>


## Counting Sort | 계수 정렬
데이터의 최대값이 K일 때 <br>
시간복잡도 : O(N + K)  
공간복잡도 : O(N + K)


- 다른 정렬 알고리즘들고 다르게 데이터끼리 비교 연산을 하지 않는다.
- 모든 데이터가 정수값을 가지면서 최소값과 최대값의 차이가 크지 않을 때 효율적이다.
- 최소값부터 최대값의 차이만큼의 리스트(또는 배열)를 0으로 초기화한다.
- 모든 데이터르 방문하며 해당 하는 인덱스 배열에 삽입한다.
- 이후 리스트의 값이 0이 아닌 인덱스 번호를 해당 값만큼 반복하여 출력한다.

<br>

![img-2](https://user-images.githubusercontent.com/65147869/233770718-e55f12f1-db0e-4003-ba71-8c75145c6d3d.gif)









<br><br>

## Time Sort
시간복잡도 : O(NlogN), Ω(N)
Python의 'sort', 'sorted' 함수의 정렬 알고리즘이다.




<br><br>

**출처**
*시간복잡도 표 : https://velog.io/@jaeyunn_15*  
*버블 정렬 : https://medium.datadriveninvestor.com/bubble-sort-in-javascript-298375020b29*  
*선택 정렬 : https://burning-camp.tistory.com/89*  
*삽입 정렬 : https://thinkdiff.net/insertion-sort-swift-db14b9a79016*  
*퀵 정렬 : https://velog.io/@yun8565*  
*합병 정렬 : https://velog.io/@yun8565*  
*계수 정렬 : https://herong.tistory.com/entry/계수정렬Counting-Sort*
