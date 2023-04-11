https://simplemips.000webhostapp.com/functional.html

▲ 우리 교수님이 만든 시뮬레이터

mips 시뮬레이터에서 step을 누르면 pc가 4씩 증가한다.

pc는 실행시키는 코드의 메모리 주소를 뜻하며, 메모리 주소의 단위는 byte이기에 4 byte씩 읽는다고 볼 수 있다.

32비트 mips 에서 word는 4 byte 이므로, 둘이 일치하는 것도 검증할 수 있다.

word가 메모리에 잘 위치했는지 확인하기 위해 pc의 값을 복사해서 memory Lookup에 붙여 넣으면

instruction code가 그 위치에 있는 것을 확인할 수 있다.

더 나아가 이를 통해 32비트 운영체제에서 프로세스가 최대 4gb의 메모리를 인식할 수 있음을 확인할 수도 있다.

pc는 32bit이므로 2^32까지 표현할 수 있고, pc는 byte를 나타내기에 인식할 수 있는 메모리는 2^32 byte다.

2^32 byte == 2^2 gb 이므로 4gb의 메모리만 인식할 수 있는 것이다.

만약 pc가 2^32를 넘어간다면 cpu가 이를 처리하지 못하기에 자기 자신에게 inturrupt(trap)를 걸 것이다. (이건 내 예상)
->걍 오버플러우 되어서 0 부터 감
