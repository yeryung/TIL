#  이분 탐색 (Binary Search)



#### 배열되어 있는 모든 데이터를 체크하는 순차 탐색이 아니라 탐색 범위를 절반씩 줄여가며 찾는 search 방법이다.





#### 이분 탐색의 주요 조건

* **정렬** (오름차순 / 내림차순 어느 한 조건이라도 만족해야 함.)





#### 이분 탐색 구현의 주요 point

* 처음과 끝 pointer 두개의 기준을 잡고 시작
* 찾고자 하는 데이터의 위치를 파악하여 판단



```python
while lt <= rt:
    mid = (lt + rt) // 2
    if a[mid] == m:
        print(mid+1)
    elif a[mid] > m:
        rt = mid - 1
    else:
        lt = mid + 1

```





#### 이분 탐색의 시간 복잡도

*  O(log n) 
* 탐색 대상을 절반으로 줄이기 때문이다.