# Docker

코드를 서버에 올렸을 때 제대로 동작하지 않음

--> 이유 : 나의 컴퓨터는 윈도우고, 서버스는 리눅스여서 environment disparity가 발생하기 때문이다.

--> 도커는 이를 해결해준다. Docker를 통해 다른 머신에서도 같은 환경을 구현할 수 있다.

#### Docker 구현 방법

* 내 컴퓨터에 도커 설치, 서버에도 도커 설치
* docker 파일 생성
* 구현하고 싶은 환경설정 (우분투, 파이썬, 깃, etc)
* docker파일을 서버, 컴퓨터에 주면 docker는 그 파일을 읽고, 필요한 것을 다운로드 받고
* docker는 해당 설정한 환경관 같은 버츄얼 컨테이너를 컴퓨터에 만든다, 또한 서버에도 필요한 것들을 다운로드 받는다.
* 컴퓨터에서 서버로 docker파일과 함께 코드를 업로드할 때 잘 작동한다.
* Docker 컨테이너는 독립적으로 분리되어 있다. -> 한 개의 서버의 다른 많은 수의 컨테이너를 가질 수 있다. (파이썬 컨테이너, 장고 컨테이너, node js 컨테이너, java 컨테이너)
* Docker 덕분에 매번 새로운 서비스를 만들 때마다 새로운 서버를 사고, 설정할 필요가 없다.
* Docker를 통해 내가 원할 때마다 새로운 환경을 생성할 수 있다. (서버를 새로 사고, 설정하고, 시작할 필요가 없다.)
* Docker를 통해 그냥 컨테이너를 생성하고 원하는 수만큼 복제하면 된다.
* 하나의 같은 서버에서 각기 다른 환경의 컨테이너를 설정할 수 있다. 또한 이 컨테이너들은 독립적으로 분리되어있다.

1. 원하는 개발 환경을 파일에 저장하면 docker는 어떤 머신에서든 해당 환경을 시뮬레이션 해준다.
2. 이러한 환경들은 각기 독립적으로 존재하므로 원하는 환경을 모듈식으로 관리 가능하다. (파이썬 서버, 자바 서버, 데이터베이스 서버를 막 추가해서 살 필요가 없다.
3. 모든 독립적 운용을 docker 하나로 가능하다.

# API

API는 애플리케이션 소프트웨어를 구축하고 통합하기 위한 정의 및 프로토콜 세트인 애플리케이션 프로그래밍 인터페이스(Application Programming Interface)를 뜻합니다.

ex) API for the tracer is torch.jit.trace() function

# TorchScript models

* TorchScript models can be saved a model archive and loaded to run in PyTorch's just-in-tim (JIT) complier instead of the CPython interpreter.
* C++ Tensor APIs support bindings to a wide range of languages and deployment environments.
* The same TorchScript models can also be loaded in the PyTorch Mobile runtime.
