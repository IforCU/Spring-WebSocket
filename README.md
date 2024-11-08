# Spring-WebSocket

## WebSocketConfig
- 스프링 스톰프를 활용하여 서버 구성
- `WebSocketConfig implements WebSocketMessageBrokerConfigurer`
  - 해당 인터페이스를 구현
- `@Configuration`
- `@EnableWebSocketMessageBroker`
  - 서버 구성 어노테이션

## WebSocketController
- `@Controller`
- `@MessageMapping("/hello")`
  - Stomp에서 사용하는 매핑 어노테이션
- `@SendTo("/topic/greetings")`
  - 해당 메서드의 결과 값을 보낼 주소 어노테이션