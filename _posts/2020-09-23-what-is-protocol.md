---
title: Protocol(프로토콜)이란?
author: Skyler Seo
date: 2020-09-23 12:55:00 +0900
categories: [dev, web]
tags: [protocol, communication-protocol]
---

통신 프로토콜 또는 통신 규약은 컴퓨터나 원거리 통신 장비 사이에서 메시지를 주고 받는 양식과 규칙의 체계이다.

통신 프로토콜은 신호 체계, 인증, 그리고 오류 감지 및 수정 기능을 포함할 수 있다.

프로토콜은 형식, 의미론, 그리고 통신의 동기 과정 등을 정의하기는 하지만 구현되는 방법은 독립적이다.

따라서 프로토콜은 하드웨어 또는 소프트웨어 그리고 때로는 모두를 사용하여 구현되기도 한다.

# 프로토콜의 예시

- [HTTP](https://ko.wikipedia.org/wiki/HTTP) : Hyper Text Transfer Protocol
- [HTTPS](https://ko.wikipedia.org/wiki/HTTPS) : Hyper Text Transfer Protocol Secure
- [FTP](https://ko.wikipedia.org/wiki/%ED%8C%8C%EC%9D%BC_%EC%A0%84%EC%86%A1_%ED%94%84%EB%A1%9C%ED%86%A0%EC%BD%9C) : File Transfer Protocol
- [SFTP](https://ko.wikipedia.org/wiki/SSH_%ED%8C%8C%EC%9D%BC_%EC%A0%84%EC%86%A1_%ED%94%84%EB%A1%9C%ED%86%A0%EC%BD%9C) : Secure File Transfer Protocol
- [Telnet](https://ko.wikipedia.org/wiki/%ED%85%94%EB%84%B7) : TErminaL NETwork
- [POP3](https://ko.wikipedia.org/wiki/POP3) : Post Office Protocol version 3
- [SMTP](https://ko.wikipedia.org/wiki/SMTP) : Simple Mail Transfer Protocol
- [SSH](https://ko.wikipedia.org/wiki/%EC%8B%9C%ED%81%90%EC%96%B4_%EC%85%B8) : Secure Shell
- [SSL](https://ko.wikipedia.org/wiki/SSL) : Secure Socket Layer
- [SOAP](https://ko.wikipedia.org/wiki/SOAP) : Simple Object Access Protocol
- [ARP](https://ko.wikipedia.org/wiki/ARP) : Adress Resolution Protocol

# 프로토콜의 구성

프로토콜은 두 가지로 이루어져 있으며 물리적 측면과 논리적 측면으로 나뉜다.

- **물리적 측면:** 자료 전송에 쓰이는 전송 매체, 접속용 단자 및 전송 신호, 회선 규격 등.
- **논리적 측면:** 프레임(Frame, 자료의 표현 형식 단위) 구성, 프레임 안에 있는 각 항목의 뜻과 기능, 자료 전송의 절차 등.
  - **폐쇄적인 프로토콜:** 자사 장치들끼리 통신하기 위한 독자적인 통신 규약이며, 자세한 규격이 공개되어 있지 않아서 크래킹 위협에 상대적으로 안전하다. (보기: IBM의 [SNA](https://ko.wikipedia.org/wiki/SNA), [SDLC 프로토콜](https://ko.wikipedia.org/w/index.php?title=SDLC_%ED%94%84%EB%A1%9C%ED%86%A0%EC%BD%9C&action=edit&redlink=1))
  - **공개된 범용 프로토콜:** 여러 장치들에 쓰이는 널리 알려진 규격이며, 규격이 널리 공개되어 있기 때문에 컴퓨터와 네트워크 크래킹에 취약한 편이다. (보기: 인터넷의 TCP/IP)

# 대표적인 프로토콜 정의 기관

- [ISO](https://ko.wikipedia.org/wiki/ISO)(International Organization for Standardization)
- [EIA](https://ko.wikipedia.org/wiki/EIA)(Electronic Industries Organization)
- [IEEE](https://ko.wikipedia.org/wiki/IEEE)(Institute of Electrical and Electronic Engineers)
- [CCITT](https://ko.wikipedia.org/w/index.php?title=CCITT&action=edit&redlink=1)(Consultative Committee for International Telegraph and Telephone)
- [IAB](https://ko.wikipedia.org/wiki/IAB)(Internet Activities Board)

## Materials

[wikipedia](https://ko.wikipedia.org/wiki/%ED%86%B5%EC%8B%A0_%ED%94%84%EB%A1%9C%ED%86%A0%EC%BD%9C#:~:text=%ED%86%B5%EC%8B%A0%20%ED%94%84%EB%A1%9C%ED%86%A0%EC%BD%9C%20%EB%98%90%EB%8A%94%20%ED%86%B5%EC%8B%A0%20%EA%B7%9C%EC%95%BD,%EC%9D%84%20%ED%8F%AC%ED%95%A8%ED%95%A0%20%EC%88%98%20%EC%9E%88%EB%8B%A4.)
