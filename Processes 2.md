# 핵심 내용
* IPC 통신의 개념
* IPC 통신의 모델
  * Shared memory
  * Message passing
    * Communication Links
      * direct / indirect
      * synchronous(blocking) / asynchronous(non-blocking)
      * automatic / explicit buffering
* IPC 통신의 예시
  * Shared memory
    * POSIX Shared Memory
  * Message passing
    * Pipes
      * Ordinary Pipes
      * Named Pipes
* Client - Server communication (Network)
  * Sockets
  * RPCs

# RPC (Remote Procedure Call)
* 원격 서버의 함수를 호출 가능
* IDL (Interface Definition Language)을 사용하여 호출 구약을 정의하고 Stub 코드를 생성
* Process 에서 Stub을 call => 네트워크 지식 없이 원격함수 호출이 가능

# Android Binder 통신
* 안드로이드 커널 (리눅스) 에서는 IPC 로 Binder 통신을 제공
* socket, pipe 등을 사용하지 않고 Binder 통신을 새로 만든 이유
