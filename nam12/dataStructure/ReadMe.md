10828 : push 입력 부분을 어떻게 처리할지 고민하다가

input().split 으로 2번 끊어서 받고 ctrl[0] 과 ctrl[1]로 구분하자.

input().split => 더 좋은 입력방법으로 바꾸어 보기.

===================================

9093 : list 슬라이싱을 최대한 이용해보자.

Python array[::] 용법
간단한 파이썬 팁입니다.
arr[::], arr[1:2:3], arr[::-1] 등으로 배열의 index에 접근하는 방법을 Extended Slices 라고 부릅니다.

설명
arr[A:B:C]의 의미는, index A 부터 index B 까지 C의 간격으로 배열을 만들어라는 말입니다.
만약 A가 None 이라면, 처음부터 라는 뜻이고
B가 None 이라면, 할 수 있는 데까지 (C가 양수라면 마지막 index까지, C가 음수라면 첫 index까지가 되겠습니다.)라는 뜻입니다.
마지막으로 C가 None 이라면 한 칸 간격으로 라는 뜻입니다.

예시

> > arr = range(10)
> > arr
> > [0,1,2,3,4,5,6,7,8,9]
> > arr[::2] # 처음부터 끝까지 두 칸 간격으로
> > [0,2,4,6,8]
> > arr[1::2] # index 1 부터 끝까지 두 칸 간격으로
> > [1,3,5,7,9]
> > arr[::-1] # 처음부터 끝까지 -1칸 간격으로 ( == 역순으로)
> > [9,8,7,6,5,4,3,2,1,0]
> > arr[::-2] # 처음부터 끝까지 -2칸 간격으로 ( == 역순, 두 칸 간격으로)
> > [9,7,5,3,1]
> > arr[3::-1] # index 3 부터 끝까지 -1칸 간격으로 ( == 역순으로)
> > [3,2,1,0]
> > arr[1:6:2] # index 1 부터 index 6 까지 두 칸 간격으로
> > [1,3,5]

출처: https://blog.wonkyunglee.io/3 [Wonkyung's blog]

===========================================================
9012 :
string을 입력받을 때

1.  string = (sys.stdin.readline().rstrip()) 2. string = (sys.stdin.readline().rstrip().split())

for char in string : 의 경우 1번은 한 글자당 끊어서 인식되고
2번의 경우 공백이 나오기 전까지를 하나의 글자로 봐서 그냥 char = string이 되버린다.

========================================================
1874 :

input을 입력받고 current와 비교한다.
cur보다 작으면 찰 때까지 +(push)해주고, 도달하면 pop한다.

# ㄴ 다시 풀어보기

==========================================================
1406 :

왜 시간초과가 뜨지??

====================================================
1158 :

for i in range(N): <= 가능  
 queue.append(i)
print(queue[i])

for i in range(1, N+1): <= 불가능 list index out of range WHY?
queue.append(i)
print(queue[i])

# ctrl + k + c....전체주석. ctrl + k + u

===============================================

10808번

아스키 코드이용하기

chr 아스키 => 문자
ord 문자 => 아스키

=========================================

11655번

isupper(), islower(), isdigit(), isspace() 함수 존재해서 사용하면됨.
