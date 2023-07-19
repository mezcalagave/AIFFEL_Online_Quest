# AIFFEL Campus Online 5th Code Peer Review Templete
- 코더 : 이영빈
- 리뷰어 : 허남철


# PRT(PeerReviewTemplate) 
각 항목을 스스로 확인하고 토의하여 작성한 코드에 적용합니다.

- [o] 코드가 정상적으로 동작하고 주어진 문제를 해결했나요?
  ![image](https://github.com/NamcheolHer/AIFFEL_Online_Quest/assets/136042769/92c7288f-c25e-46c3-80bc-41c644b8e65a)

- [o] 주석을 보고 작성자의 코드가 이해되었나요?
  네 잘이해 되었습니다.
  ![image](https://github.com/NamcheolHer/AIFFEL_Online_Quest/assets/136042769/68ff9916-e775-4aec-abde-575d162134bb)

- [o] 코드가 에러를 유발할 가능성이 없나요?
  입력값만 잘 들어 온다면 에러유발 가능성은 없습니다.
- [o] 코드 작성자가 코드를 제대로 이해하고 작성했나요?
  네 프론트 미들 테일 구간을 잘 나누어 진행하였고 코드 설명을 요청하였을때 세세한 부분까지 잘 설명하였습니다.
- [o] 코드가 간결한가요?
  > 네 주어진 task를 잘 진행할 정도로 충분히 간결합니다.
```python
import random
call_list = [1,2,3,4,5,6,7,8,9,10,11,11,12,12,13,13,14,14,15,15,16,16,17,17,18,18,19,19,20,21,22,23,24,25,26,27,28,29,30] #주머니
front_list = []
middle_list = []
tail_list = []

for i in range(20) :
  input = random.sample(call_list,1) #사회자가 부른거
  input_index = call_list.index(input[0])
  call_list.pop(input_index) #주머니에서 빼기

  if input[0] <=10:
    if len(front_list)<=5 :
      front_list.append(input[0])
      # print(front_list)
    else:
      if len(middle_list) <=10:
        middle_list.append(input[0])
      else:
        if len(tail_list) <= 5:
          tail_list.append(input[0])
  elif input[0] > 10 and input[0] <= 19:
    if len(middle_list) <= 10:
      middle_list.append(input[0])
    else:
      if len(tail_list) <= 5:
        tail_list.append(input[0])
  else:
    if len(tail_list) <= 5:
      tail_list.append(input[0]) 
```
