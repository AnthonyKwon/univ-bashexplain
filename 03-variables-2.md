# 야매로 배우는 쉘 스크립트 
### 3. 변수 (2)
변수 내에 명령어를 실행했을 때의 결과를 저장한 뒤 출력시킬 수도 있다.  
아래 예제에서는 현재 유저가 들어가 있는 그룹 목록을 출력해보겠다.

#### 코드 전문  

    #!/bin/bash
    mygroup=$(groups)
    echo "$(whoami)의 그룹: $mygroup"
    
#### 코드 해설  

    mygroup=$(groups)
    
mygroup 변수에 `groups` 명령어의 실행 결과를 저장한다

    echo "$(whoami)의 그룹: $mygroup"
    
`echo`를 통해 `whoami` 명령어의 결과물과 mygroup 변수를 **"centos의 그룹: centos wheel adm"** 과 같은 식으로 출력한다.
