OSI(Open Systems Interconnection) 7계층 모델은 네트워크의 통신을 7개의 계층으로 나누어 체계적으로 설명하기 위해 만들어진 모델이다. 각 계층은 자신만의 특정한 역할을 독립적으로 담당하며 계층 간의 상호작용을 거쳐서 데이터가 전달된다. 네트워크의 통신 방식을 표준화하는 것이 OSI 7계층의 주요 목적이다.

## 물리 계층(Physical Layer)
전기 신호나 광 신호 등과 같은 물리적 매체를 통해 데이터를 전달하는 계층이다. 케이블 등 하드웨어적인 요소와 관련이 있는 계층이다.

## 데이터 링크 계층(Data Link Layer)
CRC(Cycle Redundancy Check)를 통해 물리 계층에서 발생할 수 있는 오류를 검출하여, 네트워크 장치 간의 신뢰성 있는 데이터 전송을 보장한다. 데이터 전송은 프레임이라고 하는 단위로 쪼개어 전송하며 MAC(Media Access Control)를 통해 데이터 전송 간의 충돌을 방지한다. 데이터 링크 계층의 주요 장치로는 스위치, 브리지 등이 있다.

## 네트워크 계층(Network Layer)
서로 다른 네트워크 간에 데이터를 라우팅하여 최적의 경로로 패킷을 전송하는 계층이다. 패킷은 네트워크 계층에서 데이터가 이동되는 최소 단위를 뜻하며, 라우팅은 데이터를 목적지까지 전송하기에 최적인 경로를 찾아서 그 경로를 통해 데이터를 목적지로 전송하는 과정을 뜻한다. IP(Internet Protocol), ICMP(Internet Control Message Protocol) 등의 프로토콜을 사용하여 데이터 전송을 한다. 네트워크 계층의 주요 장치로는 라우터가 있다.

## 전송 계층(Transport Layer)
신뢰성 있는 데이터 전송을 보장하는 계층이다. 데이터는 세그먼트라는 단위로 쪼개어 전송하며, 오류 검출과 흐름 제어를 담당한다. 실제 데이터 전송 전에 TCP(Transmission Control Protocol)를 통해 안정적인 데이터 전송을 보장한다. TCP처럼 안정성은 없지만 빠르다는 장점이 있는 UDP(User Datagram Protocol) 또한 전송 계층에서 쓰이는 프로토콜이다.

## 세션 계층(Session Layer)
두 장치 간의 통신 세션을 설정하고 관리하는 계층이다. 연결 끊김 발생 시 재연결을 지원하고 세션 간의 데이터 동기화를 유지한다.

## 표현 계층(Presentation Layer)
응용 계층으로부터 애플리케이션 데이터를 전달 받고 이를 처리하거나 세션 계층이 전달한 데이터를 응용 계층이 이해할 수 있는 형태로 데이터를 변환하는 역할을 하는 계층이다. 문자 인코딩, 데이터 압축, 암호화/복호화 같은 기능을 수행한다.

## 응용 계층(Application Layer)
사용자가 직접적으로 접근하는 계층으로, 애플리케이션과의 상호작용을 담당하는 계층이다. 웹 브라우저를 생각하면 이해하기 쉽다. 사용자에게 이메일, 파일 전송, 웹 서비스 등 다양한 네트워크 서비스를 제공한다. 주요 프로토콜은 HTTP(s), FTP, SMTP가 있다.
