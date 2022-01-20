[gRPC] server / client multi gradle project

- 구조: 공통 사항은 common 폴더 안에 있고, 별도의 gradle 빌드를 통해 jar로 만든 후 server / client 프로젝트에 각각 implement
    - common 의 내용물은 spring에 관련된 내용은 없고 proto만 빌드함
- server 프로젝트와 client 프로젝트는 별도의 각각 jar을 생산하며 서로 다른 포트로 뜨게 되어 있음
- http://localhost:9091/test GET 요청  `Hello ==> test` 를 보면 성
- [관련글 방푸린](http://bangpurin.tistory.com)