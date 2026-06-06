# inflearn_study

인프런 **김영한의 스프링 핵심 원리 - 기본편**과 **스프링 MVC 1편 - 백엔드 웹 개발 핵심 기술** 학습 저장소입니다. 하나의 저장소 안에 강의별로 하위 프로젝트가 나뉘어 있습니다.

## 강의 / 학습 정보

- 플랫폼: 인프런 (김영한)
- 구성
  - `core` — 스프링 핵심 원리 - 기본편
  - `spring-mvc-1` — 스프링 MVC 1편 - 백엔드 웹 개발 핵심 기술 (`servlet`, `springmvc` 하위 프로젝트)

## 사용 기술

- Java 11 / 17 (프로젝트별 상이)
- Spring Boot (core: 3.5.3 / springmvc: 2.7.15 등)
- Spring MVC, Servlet, JSP, Thymeleaf
- Lombok, JUnit 5
- Gradle

## 학습한 내용 (코드 근거)

### core — 스프링 핵심 원리 기본편
- 객체 지향 설계와 DI: `AppConfig`, 할인 정책(`FixDiscountPolicy`/`RateDiscountPolicy`)
- 스프링 컨테이너와 빈 조회: `ApplicationContext...FindTest`
- 컴포넌트 스캔과 필터 (`scan/filter`)
- 다양한 의존관계 주입과 `@Autowired` (`autowired`)
- 빈 생명주기 콜백 (`lifecycle`)
- 빈 스코프: 싱글톤/프로토타입, 웹 스코프와 `MyLogger`/Provider (`scope`, `web`)
- 싱글톤 컨테이너와 상태 공유 문제 (`singleton`)

### spring-mvc-1 — 스프링 MVC 1편
- 서블릿 기본: 요청 파라미터/헤더, HTTP 요청·응답, JSON 처리 (`servlet/basic`)
- 직접 구현한 프론트 컨트롤러 패턴 v1~v5, 핸들러 어댑터 (`web/frontcontroller`)
- 서블릿/JSP/스프링 MVC 발전 과정 (`web/servlet`, `web/servletmvc`, `web/springmvc/v1`~`v3`)
- 스프링 MVC 기본 기능: 요청 매핑, 요청/응답 처리, 로깅 (`springmvc/basic`)
- 상품 관리 예제: `BasicItemController`, 타임리프 템플릿 (`item-service`)

## 프로젝트 구조

```
inflearn_study/
├── core/               # 스프링 핵심 원리 - 기본편
└── spring-mvc-1/       # 스프링 MVC 1편
    ├── servlet/        # 서블릿, 프론트 컨트롤러 패턴, MVC 발전 과정
    ├── springmvc/      # 스프링 MVC 기본 기능
    └── item-service/   # 상품 관리 예제 (타임리프)
```
