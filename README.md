# JavaStudy
## ㅓ머1
### ㄴ일2

*이텔릭체 별/언더바2번*
**두껍게 별 2개**
~~취소선 물결2개~~
```markdown
1. 순서가 있는 항목
1. 순서가 있는 항목
    1. 순서가 없는 항목
    1. 순서가 없는 항목
1. 순서가 있는 항목
1. 순서가 있는 항목

- 순서가 없는 항목
- 순서가 없는 항목
    - 순서가 없는 항목
    - 순서가 없는 항목

링크 문법 구조
[이름](링크)
[이름](링크 "설명")
[이름][참조]

[참조]: 링크
[참조]: 링크 "설명"

[GOOGLE](https://google.com)

[NAVER](https://naver.com "링크 설명(title)을 작성하세요.")

[상대적 참조](../users/login)

[Dribbble][Dribbble Link]

[GitHub][1]

[Dribbble Link]: https://dribbble.com
[1]: https://github.com
[참조 링크]: https://naver.com "네이버로 이동합니다!"
```
# 2025-02-12
## 수열
    - # 등비수열
        - a = 시작 값 d = 등비 n = 몇 번째인지를 나타내는 정수
        ex) 2 6 18 54 162 486 ... 2부터 시작 3곱함
        
        ```python
        def sequences(a, d, n):
            for i in range(a, n+1):
                a += d
        return a
    a, d, n = map(int, input().split())
    result = sequences(a, d, n)
    print(result)
```
    - # 등차수열
        - 1, 3, 5, 7, 9, ... 은 등차수열이다 (2씩 증가) 등차 수열 = 연속하는 두 항의 차이가 모두 일정한 수열
a= 시작하는 수 d = 수열의 공차 n = n번째 수

```python
def sequences(a, d, n):
    for i in range(a, n):
        a += d
    return a
a = int(input())
d = int(input())
n = int(input())
result = sequences(a, d, n)
print(result)
```

```python
def test(a, d, n):
    return a + (n-1) * d
```
    - # 수열
        - a = 시작 값 m = 곱할 값 d = 더할값 n = 몇 번째 인지를 나타내는 정수 (a,m,d 는 -50 ~+50, n은 10이하의 자연수)
```python
def sequences(a, m, d, n):
    for i in range(a, n):
        a = a * m + d
return a
a, m, d, n= map(int, input().split())
result = sequences(a, m, d, n)
print(result)
```
