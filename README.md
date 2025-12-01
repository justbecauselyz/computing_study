# 파이썬 공부 기록
## 2025.11.27
### print 기초
- 단어를 어떠한 특수문자로 나눌때에는 맨 뒤에 sep='/' 등으로 나타내면 됨  
input> print('naver','kakao','sk','samsung',sep=';')  
output> naver;kakao;sk;samsung
- print 줄바꿈을 하기 위해서는 줄 바꾸고 싶은 곳 맨 마지막에 end="" 추가  
ex) print('first',end="");print('second')
## 2025.12.01
### python 문자열
- 문자열은 수정 불가
- 문자열은 변경할 수 없는자료형
    - replace 메서드를 사용하면 원본은 그대로 둔 채 변경된 새로운 문자열 객체를 리턴
- 두 문자열에 대해 덧셈 기호눈 문자열의 연결을 의미
- endswith(): 정의된 문자열이 지정된 접미사로 끝나면 True로 돌려주고, 그렇지 않으면 False로 돌려줌
    ex) ex_str = "It’s been a long time!"
        ex_str.endswith('time!') or ex_str.startswith('time!')
        >>> True
### python 리스트
- list.insert(index, element)
    - list: 요소를 삽입할 리스트
    - index: 요소를 삽입할 위치의 인덱스(정수)
    - element: 삽입할 요소(어떤 자료형이든 가능)
    ex) my_list = ['apple', 'banana', 'cherry']
        <!-- 인덱스 1의 위치에 'orange' 삽입 -->
        my_list.insert(1, 'orange')
        print(my_list)
- join(리스트)
    - "".join(리스트): 매개변수로 들어온 ['a', 'b', 'c'] 이런 식의 리스트를 'abc'의 문자열로 합쳐서 반환해주는 함수
    - '구분자'.join(리스트): 리스트의 값과 값 사이에 '구분자'에 들어온 구분자를 넣어서 하나의 문자열로 합쳐줌
        ex) '_'.join(['a','b','c']): "a_b_c"와 같은 형태로 문자열을 만들어서 반환
- 리스트 정렬
    - sort(), sorted() : 오름차순 정렬
        ex) data = [2, 4, 3, 1, 5, 10, 9]
            data.sort()
            print(data)
            >>> [1, 2, 3, 4, 5, 9, 10]
