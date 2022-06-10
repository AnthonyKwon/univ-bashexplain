# 야매로 배우는 쉘 스크립트 
### 2. 변수
쉘 스크립트에서도 내부적으로 사용할 변수를 선언하거나 쉘에서 선언한 환경변수를 사용할 수 있다.  
변수에 본인의 유저명을 적고 그것을 출력하는 것을 해보겠다.  

코드 전문

    #!/bin/bash
    name="centos"
    echo "Hello, $name!"
    echo "Hello, ${name}user!"

코드 해설

    name="centos"
    
name이라는 변수를 centos라는 값으로 정의한다

    echo "Hello, $name!"
    
echo를 이용해 name의 값을 "Hello, centos!" 형태로 출력한다

    echo "Hello, ${name}user!"

echo를 이용해 name의 값을 "Hello, centosuser!" 형태로 출력한다  
  
`$name`과 `${name}`의 차이:  
`$name`의 경우 변수명의 끝이 명확하지 않기 때문에 `echo "Hello, $nameuser!"`와 같은 식으로 적을 경우,  
스크립트에서 변수명을 재대로 인식하지 못해 문제가 발생한다.  
하지만 `${name}`의 경우 중괄호로 변수가 확실히 구분되어 있으므로 위와 같은 문제가 발생하지 않는다. 
