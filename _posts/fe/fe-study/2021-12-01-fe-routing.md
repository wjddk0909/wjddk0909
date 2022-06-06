--- 
title: "라우팅 - 동적라우팅 / 정적라우팅" 
excerpt: "Routing"
categories: 
    - fe-study
tags: 
    - Routing
    - Static Routing
    - Dynamic Routing
toc: false
--- 
## 라우팅 이란?

네트워크 계층에서 길을 찾아주는 것, 즉 패킷이 목적지에 도달할 최적의 경로를 찾아 전송하는 것 -> 라우팅 테이블을 보고 길을 찾아준다. (라우팅 테이블은 나와 연결된 이쪽 인터페이스쪽으로 가면 목적지가 있겠구나를 알려줌)  

## 정적라우팅(Static Routing) vs 동적라우팅(Dynamic Routing)

- 정적라우팅 : 목적지 주소까지 어떻게 가야하는지 직접 지정

- 동적라우팅 : 목적지 주소까지 어떻게 가야하는 자동으로 지정

SPA는 최초 로드시 데이터를 전부 다운로드 하는데 이는 초기 구동시에 필요없는 데이터까지 전부 받기 때문에 오히려 처음 페이지 로드가 느려질 수 가 있다.  
그래서 초기 구동 속도 향상을 위해 동적 라우팅(또는 컴포넌트)로 component를 import 하면 (`component: () => import('컴포넌트 경로')`) 라우터 진입시에 필요한 데이터를 받아온다.  
