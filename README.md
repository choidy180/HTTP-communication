# HTTP 통신

1.1 HTTP

HTTP는 웹 브라우저와 웹 서버가 HTML로 작성된 웹 페이지나 동영상, 음성 파일 등을 주고받기 위한 프로토콜(통신 규약)입니다.
RFC2616이라는 이름으로 규정되어 있으며, 하이퍼 텍스트 프로토콜이라는 이름으로도 부릅니다.
이 프로토콜을 SSL로 암호화하여 보완성을 확보한 것을 가리켜 HTTPS라고 합니다.

1.2 HTTP 통신

HTTP에서는 클라이언트가 서버에 요청 메시지를 보내고 이에 대해 서버가 응답 메시지를 반환합니다.
서버는 응답 메시지를 반환한 후에 초기 상태로 돌아갑니다. 이때 서버는 클라이언트 상태를 저장하지 않습니다.
HTTP에서는 전송 계층 프로토콜로 TCP를 사용하고 네트워크 계층 프로토콜 IP를 사용하는 것이 일반적 입니다.
이 두 계층을 합쳐서 TCP/IP라는 이름으로 부릅니다. TCP/IP에서는 IP주소를 사용해서 통신할 컴퓨터를 결정합니다.
그리고 포트번호를 사용해서 그 컴퓨터의 어떤 프로그램과 통신할지를 결정합니다.
HTTP에서는 기본적으로 80번 포트를 사용합니다.

1.3 HTTP 요청 메시지

HTTP 요청 메시지는 다음 그림과 같이 요청 행, 요청 헤더, 메시지 본문이라는 세 부분으로 구성됩니다.
다음은 HTTP 요청 메시지의 한 부분인 요청 행의 구체적인 예입니다.
+ GET http://www.gitbut.co.kr HTTP/1.1

이 문자열은 다음과 같은 세가지 정보를 가지고 있습니다

+ GET:요청 메서드

+ http://www.gilbut.co.kr : URL

+ HTTP/1.1 : HTTP의 버전

요청 메서드는 송수신 방법을 뜻하며 GET, POST, PUT, DELETE 등이 요청 메서드에 속합니다.


웹 페이지에서는 대부분의 통신에 GET 메서드를 사용하며, 폼 등을 사용해서 데이터를 전송할 때는 POST 메서드를 사용합니다
